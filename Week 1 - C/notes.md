# CS50x – Week 1 (C)

## Source Code and the Development Environment

Source code is the human-readable version of a program.
It is written by developers using programming languages
and describes the logic and behavior of a system.

However, computers cannot execute source code directly.
It must first be transformed into a form the machine understands.

In CS50, Visual Studio Code is used as the development environment.
It provides tools to:

- write source code
- run programs
- interact with the compiler
- view output and errors

The editor itself does not execute the program.
It acts as an interface between the developer and the system.

## From Input to Output – The compilation process

Programs often follow a simple but powerful flow:
input → processing → output.

In languages like C, source code is passed to a compiler,
which translates it into machine code.

The compilation step is essential because:

- humans write code in high-level languages
- computers execute low-level instructions

Once compiled, the program can receive input,
process it according to its logic,
and produce output.

This reinforces the idea that software is a transformation
of input data into meaningful output through defined rules.

## GUI vs CLI – Different ways to interact with programs

Programs can be interacted with in different ways.

A GUI (Graphical User Interface) allows users to interact
using visual elements such as:

- buttons
- windows
- icons

A CLI (Command Line Interface) allows interaction
through text-based commands.

While GUIs are more intuitive for most users,
CLIs offer greater control, transparency, and efficiency,
especially for development and debugging.

In CS50, the CLI is emphasized because it:

- exposes how programs actually run
- makes input and output explicit
- helps understand what the computer is doing step by step

## Hello, World

"Hello, World" is usually the first program written in a new language.

Its goal is not to be complex, but to show the full flow:

- writing source code
- compiling it
- executing the program
- seeing output on the screen

Even a very small program already follows all these steps.

## Input and Output

In this example, the program does not receive input.
It only produces output.

The `printf` function sends text to standard output (the terminal).

This reinforces the idea that programs are based on:

- input
- processing
- output

## From Scratch to C

Scratch and C are very different, but the logic behind them is the same.

What changes:

- Scratch hides complexity
- C exposes details like syntax, memory and compilation

What stays the same:

- sequence
- conditionals
- loops
- variables
- input and output

C forces you to be more precise.
This helps understand how computers really work.

## Header Files

Header files provide information about functions before we use them.

For example:

- `#include <stdio.h>` tells the compiler that `printf` exists

Without header files:

- the compiler would not know the function’s name
- the program would fail to compile

Header files define:

- function signatures
- types
- constants

They do not contain the full implementation, only the interface.

## CS50 Manual Pages

CS50 provides manual pages similar to Unix `man` pages.

They are used to:

- understand how a function works
- see required header files
- learn parameters and return values

Using manual pages teaches:

- how to read documentation
- how to rely less on tutorials
- how to learn independently

Documentation is a core skill in programming.

## Hello, You

Hello, You expands Hello, World by introducing input.

The program:

- asks the user for input
- stores it in a variable
- outputs a personalized message

This introduces:

- variables
- user input
- interaction with the program

Now the program responds to the user instead of only printing text.

## Terminal Commands

The terminal (CLI) allows direct interaction with the operating system.

Common commands used in CS50:

- `ls` lists files in a directory
- `cd` changes the current directory
- `mkdir` creates a new directory
- `rm` removes files
- `clear` clears the terminal screen

Using the terminal helps understand:

- how files are organized
- how programs are executed
- how developers work without a GUI

The terminal is more powerful and precise than graphical interfaces.

## Types

In C, every variable has a type.

A type defines:

- what kind of data is stored
- how much memory is allocated
- how the data is interpreted

Examples:

- `int` stores integers
- `float` stores decimal numbers
- `char` stores a single character
- `string` stores text (CS50 abstraction)

Types matter because:

- the computer needs to know how to read the bits
- operations depend on the type
- mistakes can cause bugs or crashes

C is strict about types.
This helps prevent ambiguity but requires more care.
