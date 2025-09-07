run: lexer.out
	./ass3_22CS10043.out < ass3_22CS10043_test.c
lexer.out: lex.yy.c
	gcc -o ass3_22CS10043.out ass3_22CS10043.c
	rm  lex.yy.c
lex.yy.c:
	flex ass3_22CS10043.l
clean:
	rm lex.yy.c ass3_22CS10043.out
