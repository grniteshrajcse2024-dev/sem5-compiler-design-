# Experiment 4: Valid Variable Name Checker

A Lex/Yacc program that checks whether an identifier follows valid variable naming rules (starts with a letter/underscore, followed by alphanumerics, not a reserved keyword).

## Build & Run
```
bison -d -y valvar.y
flex valvar.l
gcc y.tab.c lex.yy.c -o valvar -lfl
./valvar
```
