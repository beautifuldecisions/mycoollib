AC_PREREQ([2.69])
AC_INIT([mycoollib], [1.0], [https://faraway.org])
AC_LANG([C])
AM_INIT_AUTOMAKE([subdir-objects -Wall -Werror foreign])

# Checks for programs.
AC_PROG_CC
AC_PROG_CPP
AM_PROG_AR
LT_INIT

# Additional feature 1

AC_ARG_VAR(ENABLE_F1, [Feature 1])

AC_ARG_ENABLE([f1],
    AS_HELP_STRING([--enable-f1], [Enable Feature 1]),
    AS_IF([test "x$enable_f1" == "xyes"], AC_DEFINE([ENABLE_F1], [1], [Feature 1]))
    )

# Additional feature 2

AC_ARG_VAR(ENABLE_F2, [Feature 2])

AC_ARG_ENABLE([f2],
    AS_HELP_STRING([--enable-f2], [Enable Feature 2]),
    AS_IF([test "x$enable_f2" == "xyes"], AC_DEFINE([ENABLE_F2], [1], [Feature 2]))
    )

# Create configured output
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile])
AC_OUTPUT
