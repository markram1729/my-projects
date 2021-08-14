LEX= flex
YACC= yacc
LIBES= -ll -w
CC = gcc

neo:    parser.l parser.y 
	$(LEX)  parser.l
	$(YACC) parser.y
	$(CC) -o neo y.tab.c $(LIBES)

.PHONY: clean    
clean:
	rm neo lex.yy.c y.tab.c
