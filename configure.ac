#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ(2.61)
AC_INIT([lemon], [0.1], [serge@vak.ru])
AM_INIT_AUTOMAKE(lemon, 0.1, no-define)
AC_CONFIG_SRCDIR([src/lemon.c])
AC_CONFIG_HEADER([config.h])
AC_CONFIG_FILES([Makefile src/Makefile examples/Makefile])

# Checks for programs.
AC_PROG_CC
AC_PROG_CXX
AC_PROG_LEX

# Checks for libraries.

# Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADERS([stdlib.h string.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_C_CONST
AC_TYPE_SIZE_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_FUNC_STRTOD
AC_FUNC_VPRINTF
AC_CHECK_FUNCS([memset strchr strrchr strtol])

AC_OUTPUT
