# CSE 230
>These are my notes

- [1.1 Compilers](#11-Compilers)


## 1.1 Compilers
Compilers
- program that translates a high level programming language into executable code 

Syntax Analysis 
- performs Syntax rules checking and constructs a symbol table and syntax tree
## 3 stages: Frontend, Middle, Backend ##
### Compiler Front End ###
- performs syntax Checking using **Lexical analyzer** and **parser**
**Lexer** - separates the input code text into recognizable language called tokens

**Syntax analyzer(parser)** - performs syntax rules checking construst a **symbol table** and **abstract syntax tree**
1. Symbol table:constructed by the execution of the **parcer** and **lexer**
- tracks the scope of the symbols in the program
2. Abstract Syntax Tree: output of the frontend
- intermediate representation of the program

### Compiler Middle-Stage ###
- performs analysis & optimization of the program
- this stage looks for common patterns that can be reorganized
- this stage also may delete unused variables or operations
- often results in smaller executables with higher performance

### Compiler Backend ###
- Arranges the symbol table in memory & generates final executable machine code
- **Linkers** :combines partial programs & Libraries into a single executable
- **Assembler** : translates assembly language code into machine
