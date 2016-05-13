
AC_INIT([noise-c], [0.0.1])
AM_INIT_AUTOMAKE

AC_PROG_CC
AC_PROG_CC_STDC
AC_PROG_RANLIB
AC_PROG_LEX
AC_PROG_YACC
AC_PATH_PROG(DOXYGEN, doxygen)

AC_CHECK_LIB(rt, clock_gettime)

dnl Try to detect winsock2 on mingw32/64 systems.
AC_CHECK_LIB(ws2_32, [_head_libws2_32_a])
AC_CHECK_LIB(ws2_32, [_head_lib32_libws2_32_a])
AC_CHECK_LIB(ws2_32, [_head_lib64_libws2_32_a])

AC_SUBST([WARNING_FLAGS],[-Wall])

AC_CONFIG_FILES([Makefile
include/Makefile
include/noise/Makefile
include/noise/protocol/Makefile
include/noise/keys/Makefile
src/Makefile
src/protocol/Makefile
src/protobufs/Makefile
src/keys/Makefile
tests/Makefile
tests/unit/Makefile
tests/vector/Makefile
tests/performance/Makefile
tools/Makefile
tools/keytool/Makefile
tools/protoc/Makefile
examples/Makefile
examples/echo/Makefile
examples/echo/echo-client/Makefile
examples/echo/echo-keygen/Makefile
examples/echo/echo-server/Makefile
doc/Makefile])
AC_OUTPUT