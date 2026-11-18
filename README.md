# C Preprocessor

## Project Overview

The **C Preprocessor** is a modular C programming project that implements basic preprocessor operations on a C source file. The executable, named `mypreprocessor`, accepts a source filename through command-line arguments and generates a processed output file with the `.i` extension.

## Objectives

The project aims to implement the following preprocessor operations:

1. **Comment Removal** – Identify and remove single-line (`//`) and multi-line (`/* ... */`) comments while preserving the readability of the remaining source code.
2. **Header File Inclusion** – Process `#include` directives by opening the specified header file and inserting its contents in place of the include directive.
3. **Macro Substitution** – Store `#define` directives and replace subsequent macro usages with their corresponding values. The requirements include simple macros and macros with arguments.

## Project Structure

```text
.
├── Makefile
├── main.c
├── preprocessor.h
├── header.h
├── commentRemoval.c
├── headerfileinclusion.c
├── macro_replacement.c
├── test.c
└── README.md
```

### File Description

- `main.c` – Main program and command-line argument handling.
- `preprocessor.h` – Common declarations and project definitions.
- `header.h` – Header file used by the project.
- `commentRemoval.c` – Comment-removal functionality.
- `headerfileinclusion.c` – Header-file inclusion functionality.
- `macro_replacement.c` – Macro substitution functionality.
- `test.c` – Test source file.
- `Makefile` – Build instructions for compiling the project.

## Compilation

Compile the project using the Makefile:

```bash
make
```

This generates the executable named:

```bash
mypreprocessor
```

## Execution

Run the preprocessor by providing a C source filename as a command-line argument:

```bash
./mypreprocessor inputfile.c
```

After successful processing, the expected output file is:

```text
inputfile.i
```

## Example

**Input command:**

```bash
./mypreprocessor test.c
```

**Expected output filename:**

```text
test.i
```

The generated `.i` file contains the processed source code according to the implemented preprocessor operations.

## Requirements

- C compiler (GCC or compatible compiler).
- Linux terminal or another environment supporting the required C compiler and Make.
- Make utility.

## Build Cleanup

If the Makefile provides a clean target, remove generated build files using:

```bash
make clean
```

## Learning Outcomes

- Working with file handling in C.
- Reading command-line arguments.
- Processing source files line by line.
- Understanding comment removal, file inclusion, and macro substitution.
- Developing a modular C application using multiple source and header files.
- Using Makefiles to automate compilation.

---

