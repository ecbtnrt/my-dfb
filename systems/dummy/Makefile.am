## Makefile.am for DirectFB/systems/dummy

INCLUDES = \
	-I$(top_srcdir)/include		\
	-I$(top_builddir)/include	\
	-I$(top_builddir)/lib		\
	-I$(top_srcdir)/lib		\
	-I$(top_srcdir)/src


internalincludedir = $(INTERNALINCLUDEDIR)/dummy

internalinclude_HEADERS = \
	dummy.h


systemsdir = $(MODULEDIR)/systems

if BUILD_STATIC
systems_DATA = libdirectfb_dummy.o
endif
systems_LTLIBRARIES = libdirectfb_dummy.la

libdirectfb_dummy_la_LDFLAGS = \
	-avoid-version	\
	-module

libdirectfb_dummy_la_SOURCES = \
	dummy.c

libdirectfb_dummy_la_LIBADD = \
	$(top_builddir)/lib/direct/libdirect.la \
	$(top_builddir)/lib/fusion/libfusion.la \
	$(top_builddir)/src/libdirectfb.la


include $(top_srcdir)/rules/libobject.make
