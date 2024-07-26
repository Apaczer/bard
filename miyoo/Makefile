TOP=..
DIRNAME=miyoo
BUILD_DIRS = 
ALL_DIRS = 
FILES = Makefile
VERSION_PROJECT = 0.12.0# see $(TOP)/include/bard_version.h
VERSION_MIYOO = m1

ALL = ipk

include $(TOP)/config/common_make_rules

ipk:	$(TOP)/bin/bard
	mkdir -p assets
	cp $(TOP)/Bard32.png ./assets/
	VERSION=$(VERSION_PROJECT)-$(VERSION_MIYOO) gm2xpkg -i -c ./pkg.cfg
	mv bard.ipk bard_$(VERSION_PROJECT)-$(VERSION_MIYOO).ipk
	rm -r ./assets
