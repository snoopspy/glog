.PHONY: all configure configure_static configure_test build install uninstall

all: configure_static build install

configure:
	cd .. && ./configure

configure_static:
	cd .. && ./configure --enable-shared=no

configure_test:
	cd .. && ./configure --prefix=$(PWD)/install

build:
	cd .. && make

install:
	cp glog.pri .. && cd .. && sudo make install
	
uninstall:
	rm -f ../glog.pri && cd .. && sudo make uninstall
