bin_PROGRAMS = exp1 exp2 exp3 exp4 exp5 exp6 dcalc
exp1_SOURCES = exp1.c
exp2_SOURCES = exp2.c
exp3_SOURCES = exp3.c
exp4_SOURCES = exp4.c
exp5_SOURCES = exp5.c lexer.l
dcalc_SOURCES = desktop_calc.cc
AM_CFLAGS = -Wall -g -O

install:

clean-local:
	-rm -rf *~ *.out example[0-9].[cdh] lexer.c

distclean-local:
	-rm -rf autom4te.cache

example1.c example1.h: example1.y
	lemon example1.y

example2.c example2.h: example2.y
	lemon example2.y

example3.c example3.h: example3.y
	lemon example3.y

example4.c example4.h: example4.y
	lemon example4.y

example5.c example5.h: example5.y
	lemon example5.y

example6.d: example6.y
	lemon -ld example6.y

exp1.o: example1.c
exp2.o: example2.c
exp3.o: example3.c
exp4.o: example4.c
exp5.o: example5.c

exp6:	example6.d
	gdc $(AM_CFLAGS) -funittest -fdebug=parser $< -o $@
