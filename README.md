# Scheme to Assembly Compiler

This repository contains the source code for a Scheme to Assembly compiler implemented in OCaml. The compiler consists of several components, including the reader, parser, semantic analysis, and code generation.

## Project Structure

The project is organized into the following components:

### Reader
- The reader module is responsible for reading Scheme source code and converting it into an internal representation suitable for parsing.

### Parser
- The parser module parses the input from the reader and constructs an abstract syntax tree (AST) representing the structure of the Scheme program.

### Semantic Analysis
- The semantic analysis module performs various checks on the AST to ensure that the program is semantically valid. This includes type checking, scope analysis, and other static checks.

### Code Generation
- The code generation module takes the validated AST and translates it into assembly language code, targeting a specific architecture or runtime environment.

### Additional Components
- In addition to the core components mentioned above, the project may include auxiliary modules for utilities, optimizations, or runtime support.

## Compilation Process

1. **Reading**: The Scheme source code is read and tokenized by the reader module.
2. **Parsing**: The token stream is parsed into an AST representing the program's structure.
3. **Semantic Analysis**: The AST undergoes semantic analysis to ensure correctness and adherence to language rules.
4. **Code Generation**: Finally, the validated AST is transformed into assembly code, ready for execution on the target platform.

## Usage

### A. To compile Scheme programs into assembly code, follow these steps:

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Build the compiler using ocmal "compiler.ml"
4. Use the compiler executable to compile Scheme source files into assembly code.

### B. To interact with the different modules of the compiler and utilize its functionality, follow these steps:

1. Launch the OCaml interpreter (utop).
2. Load the compiler.ml file by executing #use "compiler.ml";;.
3. Open the Reader module by typing open Reader;; (optinal step - depends on target moudle). 
4. You can now use the read, parse, semantic analysis, and code generation functions by calling them with the appropriate expressions as arguments. For example, execute read "your_scheme_expression";; to see the output of the reader for a Scheme expression. Similarly, you can use parse, sem, and code_gen functions in a similar manner.
