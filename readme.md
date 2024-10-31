# 🛠️ Compiler Construction Project

This repository contains the code for a compiler built as part of the **Compiler Construction** course. The project is implemented in **OCaml** and includes various components such as lexical analysis, parsing, and code generation.

## 📋 Project Overview

The compiler project is divided into two main assignments and a final project:

| Assignment | Description |
|------------|-------------|
| **Assignment 1** | Implement basic lexical analysis and parsing features by replacing instances of `raise (X_not_yet_implemented "hw 1")` with the appropriate code. |
| **Assignment 2** | Extend the functionality by replacing instances of `raise (X_not_yet_implemented "hw 2")` to handle more complex parsing and compilation tasks. |
| **Final Project** | Generate x86 assembly code for Scheme source programs. This stage involves writing assembly code and testing it on an Intel x86 machine with Linux ABI compatibility. |

## 📂 File Structure

- **`compiler.ml`**: The primary OCaml file containing the skeleton code for the compiler. Sections are marked to indicate where to implement functionality for each assignment and the final project.
- **`makefile`**: Used to assemble and link generated assembly files.

## 🧪 Compilation and Testing

- **`compile_scheme_string`**: Compiles Scheme source code directly into an assembly file.
- **`compile_and_run_scheme_string`**: A convenient function that compiles, assembles, and runs a Scheme string, providing immediate feedback for debugging.

### Example Usage

```ocaml
Code_Generation.compile_and_run_scheme_string "testing/goo" "(+ 2 3)"
