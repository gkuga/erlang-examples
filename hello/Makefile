MODULES = main

all: compile

compile:
	@erlc $(MODULES:=.erl)

clean:
	@rm -f $(MODULES:=.beam)

run: compile
	@erl -noshell -s $(MODULES) main -s init stop
