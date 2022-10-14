cmake_minimum_required(VERSION 3.16)
project(O2AnalysisBuildTest)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "workflows")
set(CMAKE_CXX_STANDARD 17)

find_package(O2 CONFIG REQUIRED)

ADD_EXECUTABLE(mytest o2DummyWorkflow.cxx)

TARGET_LINK_LIBRARIES(mytest O2::Framework)

