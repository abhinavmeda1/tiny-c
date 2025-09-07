run:  tinyC2_22CS10043.out
	./tinyC2_22CS10043.out < input_22CS10043.c > output_22CS10043.txt

tinyC2_22CS10043.out: all

all:
	yacc -d tinyC2_22CS10043.y 
	lex tinyC2_22CS10043.l
	gcc -g -o tinyC2_22CS10043.out tinyC2_22CS10043.c

couterexamples:
	yacc -d -Wcounterexamples tinyC2_22CS10043.y 	

clean:
	rm lex.yy.c y.tab.c y.tab.h *.out
