#############################<--OGI-->######################################
##                                                                        ##
##             Center for Spoken Language Understanding                   ##
##        Oregon Graduate Institute of Science & Technology               ##
##                         Portland, OR USA                               ##
##                        Copyright (c) 2000                              ##
##                                                                        ##
##      This module is not part of the CSTR/University of Edinburgh       ##
##               release of the Festival TTS system.                      ##
##                                                                        ##
##  In addition to any conditions disclaimers below, please see the file  ##
##  "license_ogi_tts.txt" distributed with this software for information  ##
##  on usage and redistribution, and for a DISCLAIMER OF ALL WARRANTIES.  ##
##                                                                        ##
#############################<--OGI-->######################################
##  OGIcommon - objects & function shared between various synthesis methods
############################################################################
TOP=../../../..
DIRNAME=src/modules/OGIModules/OGIcommon

LIB_BUILD_DIRS = inst_tmpl
BUILD_DIRS = $(LIB_BUILD_DIRS)

H = OGI_Buffer.h OGI_file.h OGI_Filter.h OGI_LPC.h OGI_Macro.h OGI_SingleTrack.h OGI_TimeWarp.h \
OGI_Track.h OGI_Vector.h OGI_Wave.h OGI_WaveChunk.h OGIcommon.h OGIduration.h OGIgain.h OGIpitch.h OGI_Math.h

TSRCS = OGI_Vector.cc OGI_Track_file.cc

CPPSRCS = OGI_LPC.cc OGI_file.cc OGI_TimeWarp.cc OGIcommon.cc OGI_Track.cc \
OGI_WaveChunk.cc OGIduration.cc OGI_Buffer.cc OGIpitch.cc OGIgain.cc OGI_Filter.cc  OGI_Math.cc $(TSRCS)

SRCS = $(CPPSRCS)

OBJS = $(SRCS:.cc=.o)
 
FILES = Makefile $(SRCS) $(H)
 
LOCAL_INCLUDES = -I../../../src/include
LOCAL_DEFINES = -DTMATRIX_BOUNDS_CHECKING=0


INLIB = $(TOP)/src/lib/libFestival.a
 
ALL = .buildlib
 
include $(TOP)/config/common_make_rules

