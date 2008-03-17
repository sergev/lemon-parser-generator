bin_PROGRAMS = lemon
lemon_SOURCES = lemon.c
AM_CFLAGS = -Wall -g -O -fno-strict-aliasing

clean-local:
	-rm -rf *~

distclean-local:
	-rm -rf autom4te.cache

install-data-local: ${datadir}/lemon/skeleton.c ${datadir}/lemon/skeleton.d

${datadir}/lemon/skeleton.c: skeleton.c
	${install_sh_DATA} $< $@

${datadir}/lemon/skeleton.d: skeleton.d
	${install_sh_DATA} $< $@
