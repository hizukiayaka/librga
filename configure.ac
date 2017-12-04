#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([librga], m4_esyscmd([build-aux/git-version-gen .tarball-version]), [https://github.com/hizukiayaka/librga/issues])
AM_INIT_AUTOMAKE([-Wno-portability 1.14 no-dist-gzip dist-xz tar-ustar subdir-objects])

AC_CONFIG_HEADERS([config.h])
PKG_INSTALLDIR

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
LT_INIT

# Checks for libraries.
# FIXME: Replace `main' with a function in `-ldrm':
#AC_CHECK_LIB([drm], [main])
PKG_CHECK_MODULES(DRM, libdrm)

# Checks for header files.
AC_CHECK_HEADERS([fcntl.h stdint.h stdlib.h string.h sys/ioctl.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE
AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT64_T
AC_TYPE_SIZE_T
AC_TYPE_UINT16_T
AC_TYPE_UINT32_T

# Checks for library functions.
AC_CHECK_FUNCS([malloc memset munmap strerror])

AC_CONFIG_FILES([Makefile
lib/Makefile
lib/normal/Makefile
librk_rga.pc
])

AC_OUTPUT
