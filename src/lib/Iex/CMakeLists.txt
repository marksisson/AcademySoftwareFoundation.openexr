# SPDX-License-Identifier: BSD-3-Clause
# Copyright (c) Contributors to the OpenEXR Project.

openexr_define_library(Iex
  PRIV_EXPORT IEX_EXPORTS
  CURDIR ${CMAKE_CURRENT_SOURCE_DIR}
  SOURCES
    IexBaseExc.cpp
    IexThrowErrnoExc.cpp
    IexMathFloatExc.cpp
    IexMathFpu.cpp
  HEADERS
    IexBaseExc.h
    IexMathExc.h
    IexThrowErrnoExc.h
    IexErrnoExc.h
    IexMacros.h
    IexMathFloatExc.h
    IexMathIeeeExc.h
    Iex.h
    IexNamespace.h
    IexExport.h
    IexForward.h
  DEPENDENCIES
    OpenEXR::Config
  )
