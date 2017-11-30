SUBDIRS = normal

lib_LTLIBRARIES = librk_rga.la
librk_rga_la_CXXFLAGS = $(AM_CPPFLAGS) $(DRM_CFLAGS) -I$(top_srcdir)/inc
librk_rga_la_SOURCES = RgaApi.cpp RockchipRga.cpp
librk_rga_la_LDFLAGS = -no-undefined -version-info 0:2:0
librk_rga_la_LIBADD = normal/librk_rganormal.la $(DRM_LIBS)
