cmake_minimum_required(VERSION 3.1)
project(libfm_1_42_src)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    src/fm_core/fm_data.h
    src/fm_core/fm_model.h
    src/fm_core/fm_sgd.h
    src/libfm/src/Data.h
    src/libfm/src/fm_learn.h
    src/libfm/src/fm_learn_mcmc.h
    src/libfm/src/fm_learn_mcmc_simultaneous.h
    src/libfm/src/fm_learn_sgd.h
    src/libfm/src/fm_learn_sgd_element.h
    src/libfm/src/fm_learn_sgd_element_adapt_reg.h
    src/libfm/src/relation.h
    src/libfm/tools/convert.cpp
    src/libfm/tools/transpose.cpp
    src/libfm/libfm.cpp
    src/util/cmdline.h
    src/util/fmatrix.h
    src/util/matrix.h
    src/util/memory.h
    src/util/random.h
    src/util/rlog.h
    src/util/smatrix.h
    src/util/util.h
    history.txt
    license.txt
    readme.pdf)

add_executable(libfm_1_42_src ${SOURCE_FILES})