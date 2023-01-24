# Shell

Implementing a mini shell to execute some simple shell commands.

## Run the program

```bash
make
./shell
ls -al
```
## Functions implemented
1. ls: to list all the files in a directory.
2. cat: to read the content of a file.
3. exit: instead of ctrl C to exit from the shell
4. piping: piping is implemented to pass the output of a command as input to another.
5. wildcarding: The "*" character matches 0 or more nonspace characters. The "?" character matches one nonspace character.

```bash
ls
ls -al
ls -al > out
ls -al >> out
cat out
cat < out
cat < out > out2
ls /tt >>& out2
ls -al | grep command
ls -al | grep command | grep command.o
ls -al | grep command | grep command.o > out
echo *.cc
```

## Parsing input

The input is parsed using Lex and Yacc.
