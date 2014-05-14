CC = gcc
RM = rm -rf


default:hello.c 
	$(CC) $^ -o $@

scoping_issue:
	$(call parent,one,two)

clean:default
	$(RM) $<

define parent
	@echo "parent has two parameters: $1, $2"
 	$(call child,$1)
endef

define child
	@echo "child has one parameter: $1"
endef

