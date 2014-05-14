OBJDIR = ../obj

VPATH = $(OBJDIR)

%.o : %.c
	$(COMPILE.c) $< -o $(OBJDIR)/$@

all: foo

foo: foo.o bar.o
	$(LINK.o) $^ $(LDLIBS) -o $(OBJDIR)/$@
