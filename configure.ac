 # Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
#
# Everyone is permitted to copy and distribute verbatim copies
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

# Makefile.am inspired from bison configure.ac


# file created  by Tom SCHNEIDER <dev.tomschneider@gmail.com>
# file modified by ...




AC_INIT([bumdd], [0.1.0])
[DEVEL=0]
dnl Always update all your software there is no acual need for 2.69 still !!
AC_PREREQ([2.69])

dnl #AM_SILENT_RULES([yes])
AC_CONFIG_HEADERS([lib/config.h:lib/config.in.h])

# compiler option
# Checks for the compiler.
AC_PROG_CC_STDC
AC_PROG_CXX
AC_LANG([C])
AC_LANG([C++])


# required programs for testing
[if test $DEVEL -eq 0; then]
AC_CHECK_PROGS([VALGRIND], [valgrind])
AC_CHECK_PROGS([GDB], [gdb])
AC_CHECK_PROGS([QUEMU], [QUEMU-])
[fi]

AC_CONFIG_SRCDIR([src/main.cc])
AM_INIT_AUTOMAKE

AC_CONFIG_FILES([Makefile])

AC_PROG_CXX

AC_OUTPUT
