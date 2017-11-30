AM_CFLAGS = -I$(top_srcdir)/inc
AM_CPPFLAGS = -I$(top_srcdir)/inc

BUILT_SOURCES = $(top_srcdir)/.version
$(top_srcdir)/.version:
	echo $(VERSION) > $@-t && mv $@-t $@
dist-hook:
	echo $(VERSION) > $(distdir)/.tarball-version

SUBDIRS = lib tests

rk_rga_include_HEADERS = inc/drmrga.h			\
			 inc/rga.h			\
			 inc/RgaApi.h			\
			 inc/RockchipRga.h		\
			 inc/RockchipRgaMacro.h

rk_rga_includedir = $(includedir)/rk_rga
