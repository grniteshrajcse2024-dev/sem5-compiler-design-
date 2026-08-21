# Experiment 6: Calculator using Lex/Yacc

A simple calculator that evaluates arithmetic expressions with +, -, *, /, unary minus, and correct operator precedence, built using Lex for tokenizing and Yacc for parsing.

## Build & Run
```
bison -d -y cal.y
flex cal.l
gcc y.tab.c lex.yy.c -o cal -lfl -lm
./cal
```

Example:
```
$ echo "3+4*2" | ./cal
Answer: 11
```
