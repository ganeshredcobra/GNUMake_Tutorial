SUBDIRS = foo bar src obj

default:
	gcc hello.c -o hello
subsystem:
	cd src && $(MAKE)

subdirs:
	for dir in $(SUBDIRS); do \
		$(MAKE) -C $$dir; \
	done
