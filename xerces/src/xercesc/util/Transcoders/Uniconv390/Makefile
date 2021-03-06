#
# Licensed to the Apache Software Foundation (ASF) under one or more
# contributor license agreements.  See the NOTICE file distributed with
# this work for additional information regarding copyright ownership.
# The ASF licenses this file to You under the Apache License, Version 2.0
# (the "License"); you may not use this file except in compliance with
# the License.  You may obtain a copy of the License at
# 
#      http://www.apache.org/licenses/LICENSE-2.0
# 
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
#
#
# $Log$
# Revision 1.4  2004/09/08 13:56:46  peiyongz
# Apache License Version 2.0
#
# Revision 1.3  2004/07/09 16:30:05  peiyongz
# Build on HP-Itanium, aCC A.05.52
#
# Revision 1.2  2004/02/06 15:02:41  cargilld
# Intrinsic transcoding support for 390.
#
# Revision 1.1  2002/11/22 14:57:05  tng
# 390: Uniconv390 support.  Patch by Chris Larsson and Stephen Dulin.
#
#

PLATFORM = LINUX
CC  = gcc
CXX = g++
CXXVER = 
CXXFLAGS =   -w -O2 -DNDEBUG -DPROJ_XMLPARSER  -DPROJ_XMLUTIL  -DPROJ_PARSERS  -DPROJ_SAX4C  -DPROJ_SAX2  -DPROJ_DOM -DPROJ_DEPRECATED_DOM -DPROJ_VALIDATORS -DXML_USE_NATIVE_TRANSCODER -DXML_USE_INMEM_MESSAGELOADER -DXML_USE_PTHREADS   
CFLAGS =   -w -O2 -DNDEBUG -DPROJ_XMLPARSER  -DPROJ_XMLUTIL  -DPROJ_PARSERS  -DPROJ_SAX4C  -DPROJ_SAX2  -DPROJ_DOM -DPROJ_DEPRECATED_DOM -DPROJ_VALIDATORS -DXML_USE_NATIVE_TRANSCODER -DXML_USE_INMEM_MESSAGELOADER -DXML_USE_PTHREADS    
PREFIX = /usr/local
PREFIX_INCLUDE = ${PREFIX}/include/xercesc
LDFLAGS =    
LIBS =   -lpthread 
OSVER = 
USELIBWWW = 
MESSAGELOADER = INMEM
TRANSCODER = NATIVE
THREADS = pthread
LIBTYPE = shared
ARCH = x86_64

MODULE = util
SUBMODULE = Transcoders/Uniconv390

include ../../../Makefile.incl

CPP_PUBHEADERS = Uniconv390TransService.hpp uniconv.h \
        XML256TableTranscoder390.hpp \
        XML88591Transcoder390.hpp \
        XMLASCIITranscoder390.hpp \
        XMLEBCDICTranscoder390.hpp \
        XMLIBM1047Transcoder390.hpp \
        XMLIBM1140Transcoder390.hpp \
        XMLUTF8Transcoder390.hpp \
        XMLWin1252Transcoder390.hpp

CPP_OBJECTS = Uniconv390TransService.$(TO) uniconv.$(TO) \
        XML256TableTranscoder390.$(TO) \
        XML88591Transcoder390.$(TO) \
        XMLASCIITranscoder390.$(TO) \
        XMLEBCDICTranscoder390.$(TO) \
        XMLIBM1047Transcoder390.$(TO) \
        XMLIBM1140Transcoder390.$(TO) \
        XMLUTF8Transcoder390.$(TO) \
        XMLWin1252Transcoder390.$(TO) \
        trot.$(TO) \
        ascii.$(TO)

include ../../Makefile.util.submodule
