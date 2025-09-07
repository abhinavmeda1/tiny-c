.SUFFIXES:

TinyC3_22CS10043.out: TinyC3_22CS10043_translator.cpp lex.yy.c y.tab.c y.tab.h
	g++ -o TinyC3_22CS10043.out TinyC3_22CS10043_translator.cpp

y.tab.c: TinyC3_22CS10043.y
	yacc -dv TinyC3_22CS10043.y

y.tab.h: TinyC3_22CS10043.y
	yacc -dv TinyC3_22CS10043.y

lex.yy.c:
	lex TinyC3_22CS10043.l

couterexamples:
	yacc -d -Wcounterexamples TinyC3_22CS10043.y 	

clean:
	- rm -rf lex.yy.c y.tab.c y.tab.h TinyC3_22CS10043.out y.output Output

test: TinyC3_22CS30027_22CS30019.out
	mkdir -p Output
	./TinyC3_22CS10043.out < ./Input/TinyC3_22CS10043_test1.c > ./Output/TinyC3_22CS10043_quads1.out
	./TinyC3_22CS10043.out < ./Input/TinyC3_22CS10043_test2.c > ./Output/TinyC3_22CS10043_quads2.out
	./TinyC3_22CS10043.out < ./Input/TinyC3_22CS10043_test3.c > ./Output/TinyC3_22CS10043_quads3.out
	./TinyC3_22CS10043.out < ./Input/TinyC3_22CS10043_test4.c > ./Output/TinyC3_22CS10043_quads4.out
	./TinyC3_22CS10043.out < ./Input/TinyC3_22CS10043_test5.c > ./Output/TinyC3_22CS10043_quads5.out
