# Experiment 3: Arithmetic Expression Parser

A Lex/Yacc based parser that recognizes and evaluates arithmetic expressions with standard operator precedence (+, -, *, /).

## Build & Run
```
bison -d -y art_expr.y
flex art_expr.l
gcc y.tab.c lex.yy.c -o art_expr -lfl
./art_expr
```
