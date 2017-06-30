AM_CPPFLAGS = -fno-exceptions -fno-rtti -ansi -DPOSIX

noinst_LIBRARIES = libutp.a
libutp_a_SOURCES = utp_api.cpp utp_callbacks.cpp utp_hash.cpp utp_internal.cpp utp_packedsockaddr.cpp utp_utils.cpp
libutp_a_DEPENDENCIES = $(builddir)/include/libutp
noinst_HEADERS = libutp_inet_ntop.h utp_callbacks.h utp.h utp_hash.h utp_internal.h utp_packedsockaddr.h utp_templates.h utp_types.h utp_utils.h
EXTRA_DIST = CMakeLists.txt LICENSE README.md libutp_inet_ntop.cpp

$(builddir)/include/libutp:
	$(MKDIR_P) $(builddir)/include
	(cd $(builddir)/include && $(LN_S) $(abs_srcdir) libutp)
