##===- lib/Support/Makefile --------------------------------*- Makefile -*-===##
#
#                     The LLVM Compiler Infrastructure
#
# This file is distributed under the University of Illinois Open Source
# License. See LICENSE.TXT for details.
#
##===----------------------------------------------------------------------===##

LEVEL = ../..
LIBRARYNAME = LLVMSupport
BUILD_ARCHIVE = 1

EXTRA_DIST = Unix Win32 README.txt

include $(LEVEL)/Makefile.common

CompileCommonOpts := $(filter-out -pedantic,$(CompileCommonOpts))
CompileCommonOpts := $(filter-out -Wno-long-long,$(CompileCommonOpts))

ifdef LLVM_VERSION_INFO
CompileCommonOpts += -DLLVM_VERSION_INFO='"$(LLVM_VERSION_INFO)"'
endif
ifdef CLANG_VENDOR
CompileCommonOpts += -DCLANG_VENDOR='"$(CLANG_VENDOR)"'
endif
