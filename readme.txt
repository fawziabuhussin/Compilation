# Compiler Construction Project

This repository contains the code for a compiler built as part of the Compiler Construction course assignments. The project is implemented in OCaml and includes various components like lexical analysis, parsing, and code generation.

## Project Overview

The compiler is structured across two main assignments and a final project:

1. **Assignment 1**: Focuses on replacing instances of `raise (X_not_yet_implemented "hw 1")` with appropriate code to implement lexical analysis and parsing features in OCaml.
2. **Assignment 2**: Continues the development by replacing `raise (X_not_yet_implemented "hw 2")` statements, expanding functionality to handle advanced parsing and compilation tasks.
3. **Final Project**: Involves generating x86 assembly code for Scheme source programs. This part requires developing and testing assembly code on an Intel x86 machine with Linux ABI compatibility.

## File Structure

- `compiler.ml`: The main OCaml file containing the bulk of the compiler’s skeleton code. Clearly marked sections indicate where code needs to be implemented for each assignment and the final project.
- `makefile`: Used for assembling and linking generated assembly files.

## Compilation and Testing

- Use the function `compile_scheme_string` to compile Scheme source directly to an assembly file.
- The `compile_and_run_scheme_string` function provides a convenient method to compile, assemble, and run a Scheme string, enabling fast feedback for debugging.

### Example Usage

```ocaml
Code_Generation.compile_and_run_scheme_string "testing/goo" "(+ 2 3)";;
