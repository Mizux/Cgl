# Copyright (C) 2006 International Business Machines and others.
# All Rights Reserved.
# This file is distributed under the Eclipse Public License.

## $Id: Makefile.am 1040 2011-08-14 10:49:48Z stefan $

# Author:  Andreas Waechter           IBM    2006-04-13

AUTOMAKE_OPTIONS = foreign

include $(top_srcdir)/BuildTools/Makemain.inc

########################################################################
#                          libCglGMI                              #
########################################################################

# Name of the library compiled in this directory.  We don't want it to be
# installed since it will be collected into the libCgl library
noinst_LTLIBRARIES = libCglGMI.la

# List all source files for this library, including headers
libCglGMI_la_SOURCES = \
	CglGMI.cpp  CglGMI.hpp \
	CglGMIParam.cpp  CglGMIParam.hpp

# This is for libtool (on Windows)
libCglGMI_la_LDFLAGS = $(LT_LDFLAGS)

# Here list all include flags, relative to this "srcdir" directory.
AM_CPPFLAGS = -DCGL_BUILD $(CGLLIB_CFLAGS)

########################################################################
#                Headers that need to be installed                     #
########################################################################

# Here list all the header files that are required by a user of the library,
# and that therefore should be installed in pkgincludedir.

includecoindir = $(pkgincludedir)
includecoin_HEADERS = CglGMI.hpp CglGMIParam.hpp
