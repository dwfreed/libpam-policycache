AC_PREREQ([2.68])
AC_INIT([libpam-policycache], [0.1], [https://goto.google.com/goobuntu-bug])
AC_CONFIG_AUX_DIR([autotools])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AM_SILENT_RULES([yes])

# Checks for programs.
AC_PROG_CC
AC_PROG_CC_STDC
AM_PROG_CC_C_O

# Checks for libraries.
LT_INIT
PKG_CHECK_MODULES([GLIB], [glib-2.0 >= 2.32.4])

# Checks for header files.
AC_CHECK_HEADERS([stdint.h stdlib.h string.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_UINT32_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_CHECK_FUNCS([memset])

AC_CONFIG_FILES([Makefile
                 testdata/Makefile
                 src/Makefile])
AC_OUTPUT
