## Makefile.am for DirectFB/inputdrivers/ucb1x00_ts

INCLUDES = \
	-I$(top_srcdir)/include	\
	-I$(top_builddir)/lib	\
	-I$(top_srcdir)/lib	\
	-I$(top_srcdir)/src

input_LTLIBRARIES = libdirectfb_ucb1x00_ts.la

if BUILD_STATIC
input_DATA = $(input_LTLIBRARIES:.la=.o)
endif

inputdir = $(MODULEDIR)/inputdrivers

libdirectfb_ucb1x00_ts_la_SOURCES =	\
	ucb1x00_ts.c

libdirectfb_ucb1x00_ts_la_LDFLAGS = \
	-module			\
	-avoid-version		\
	$(DFB_LDFLAGS)

libdirectfb_ucb1x00_ts_la_LIBADD = \
	$(top_builddir)/lib/direct/libdirect.la \
	$(top_builddir)/src/libdirectfb.la


include $(top_srcdir)/rules/libobject.make
	
