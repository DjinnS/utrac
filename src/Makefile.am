CHARMAPS_FILE = charsets.dat

sharedir = $(datadir)/utrac/

bin_PROGRAMS = utrac
utrac_SOURCES = 		\
	debug.h				\
	ut_charset.h		\
	ut_error.h			\
	ut_text.h			\
	utrac.h				\
	ut_conversion.c		\
	ut_loading.c		\
	ut_messages_en.c	\
	ut_recognition1.c	\
	ut_recognition2.c	\
	ut_utils.c			\
	utrac.c				\
	utrac_cmd.c

dist_check_SCRIPTS = merge.pl

utrac_LDADD = libut_charset.a

noinst_LIBRARIES = libut_charset.a
libut_charset_a_SOURCES = ut_charset.c
libut_charset_a_CFLAGS = -Wno-multichar -DUT_CHARMAPS_FILENAME='"${sharedir}${CHARMAPS_FILE}"'

man_MANS = utrac.1
dist_man_MANS = utrac.1

share_DATA = charsets.dat

EXTRA_DIST = $(share_DATA)
