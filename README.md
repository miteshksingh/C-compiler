# C-Compiler


A Small C Compiler which can handle simple sorting programs. This is just a basic compiler for preliminary anaysis of all phases of Compiler Design. The .l file generates tokens from input C program and passes to .y file which deals with the Syntactic and Semantic phases.An Intermediate Code is generated.This Intermediated Code is then stored in Quadruple Table. All Statements from Quadruple table are Converted into Assembly Instructions in GCC AT&T Syntax.This generates .s file which can be successfully executed to give desired output of input program.

Dependencies:Flex(Lecaical Analyser),Bison(Parser Generator Tool)

How to execute:

1.Install flex and Bison and set their path.

2.flex Compiler.l

3.bison Compiler.y

4.gcc Compiler.tab.c

5.a.exe .c .i .s

6.gcc -m32 .s

7.a.exe

Output:

The output will print all the grammer rules needed to parse the input C program. A Symbol table containing all variables is displayed. A Quadruple table used in generating intermediate code is also displayed. The Output of input C program is displayed.

The constructs supported by the compiler are

1.Simple Variable declaration and initialization.

2.Any Dimension Array declaration and initialization. (Error on Redeclaration,Undeclaration,Dimension Mismatch,etc.)

3.If Else Constructs

4.While Loop Constucts(Simple Sorting Programs)
