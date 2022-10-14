cmake_minimum_required(VERSION 3.16)
project(O2AnalysisBuildTest)
set(CMAKE_CXX_STANDARD 17)
set(Microsoft.GSL_DIR /home/arczipt/alice/sw/ubuntu2004_x86-64/ms_gsl/4.0.0-3/share)

find_package(O2 CONFIG REQUIRED)

ADD_EXECUTABLE(mytest o2DummyWorkflow.cxx)

TARGET_LINK_LIBRARIES(mytest O2::Framework)

