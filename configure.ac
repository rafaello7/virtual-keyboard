AC_PREREQ([2.69])
AC_INIT([virtual-keyboard], [0.5.1], [fatwildcat@gmail.com])
AM_INIT_AUTOMAKE([-Wall -Werror foreign])
AC_CONFIG_SRCDIR([src/keyboard_layout.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CC

# Checks for libraries.
AC_CHECK_LIB([X11], [XGetKeyboardMapping])
AC_CHECK_LIB([Xtst], [XTestFakeKeyEvent])
PKG_CHECK_MODULES(LIBGTK, [gtk+-3.0])

# Checks for header files.
AC_CHECK_HEADERS([stdlib.h string.h])

# Checks for typedefs, structures, and compiler characteristics.

# Checks for library functions.
AC_CHECK_FUNCS([strchr strtoul])

AC_CONFIG_FILES([Makefile src/Makefile icons/Makefile debian/Makefile])
AC_OUTPUT
