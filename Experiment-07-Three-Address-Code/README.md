# Experiment 7: Three Address Code Generation

Generates three-address code (TAC) for simple assignment statements involving arithmetic expressions, using Lex/Yacc with string-valued semantic actions to build temporaries.

## Build & Run
```
bison -d -y tac.y
flex tac.l
gcc y.tab.c lex.yy.c -o tac -lfl
./tac
```

Example:
```
$ echo "a = b + c * d" | ./tac
t1 = c * d
t2 = b + t1
a = t2
```
