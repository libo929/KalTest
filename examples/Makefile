########################################################################	
##
## ---------------------------
##   Makefile for KalTest
## ---------------------------
##
## (Version Information)
##   Version: 0.2
##   Release: 1
##
## (Update Record)
##    2002/01/18  K.Hoshina     Derived from baby/src/Makefile
##    2002/10/21  K.Fujii       Cleanup.
##
## (Description)
##   In order to use this package you should first set some
##   environmental variables. Take a look at README in the
##   top directory.
##
## (Targets)
##	all       	: builds test programs
##	Makefiles 	: creates Makefiles.
##	clean     	: deletes *.o ...
##	distclean 	: deletes even test programs.
## 
########################################################################	

MFLAGS	=
CURRDIR	= .

SUBDIRS	= kaltest

all:
	@case '${MFLAGS}' in *[ik]*) set +e;; esac; \
	for i in $(SUBDIRS); do \
	(cd $$i; echo ``making'' all ``in $(CURRDIR)/$$i...''; \
	$(MAKE) $(MFLAGS)); \
	done
	
clean:
	@case '${MFLAGS}' in *[ik]*) set +e;; esac; \
	for i in $(SUBDIRS); do \
	(cd $$i; echo ``making'' clean ``in $(CURRDIR)/$$i...''; \
	$(MAKE) $(MFLAGS) clean); \
	done

distclean: clean
	@case '${MFLAGS}' in *[ik]*) set +e;; esac; \
	for i in $(SUBDIRS); do \
	(cd $$i; echo ``making'' distclean ``in $(CURRDIR)/$$i...''; \
	$(MAKE) $(MFLAGS) distclean); \
	done; \

