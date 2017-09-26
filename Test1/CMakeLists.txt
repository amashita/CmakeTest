cmake_minimum_required(VERSION 2.6)

project(Test1)

# コンパイルオプションの指定
set( CMAKE_C_FLAGS "-Wall -g" )

# GLOB SRCSがわからないけど
# フォルダにある.cpp .hppのつくファイルを指定してることはわかる
file( GLOB SRCS *.cpp *.hpp )

# プロジェクト内でのsrcフォルダの名前
add_executable ( Test1 ${SRCS} )