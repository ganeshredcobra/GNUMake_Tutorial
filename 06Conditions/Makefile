CC = gcc
RM = rm -rf
AVR = avr-gcc

FIRST = 23
SECOND = 33

default:hello.c
ifndef AVR
	@echo No AVR
else 
	$(CC) $^ -o $@
endif

equal:
ifeq ($(FIRST),$(SECOND))
	@echo Two Variables are equal
else
	@echo Variable not equal
endif
clean:default
	$(RM) $<
