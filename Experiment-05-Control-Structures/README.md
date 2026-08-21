# Experiment 5: Control Structures Parser

A Lex/Yacc based parser that recognizes common control structures (if-else, while, for) in a simplified C-like grammar.

## Build & Run
```
bison -d -y control.y
flex control.l
gcc y.tab.c lex.yy.c -o control -lfl
./control
```
