# Stack Implementation using Linked List (PImpl Idiom)

## Overview
This project implements a **Stack** (Last-In-First-Out data structure) using a **linked list**, following the **PImpl (Pointer to Implementation) idiom**. This technique separates the **interface** (`STACK.h`) from the **implementation** (`STACK.cpp`), improving code encapsulation and maintainability.

## Features
- ✅ Stack operations: `push()`, `pop()`, `top()`, `isEmpty()`, `size()`, `clear()`
- ✅ Operator overloading (`+=`, `--`, `!`, `==`, `!=`, `>`, `<`, `<<`)
- ✅ Memory management using **smart pointers** (`std::unique_ptr`)
- ✅ Move semantics for efficient object handling
- ✅ **Custom exception handling** (`StackUnderflowException`)
- ✅ **Automated testing system** (`test.cpp`) with a log file (`log.txt`)

## Project Structure
```
📂 StackProject
├── 📜 STACK.h         # Stack class declaration (interface)
├── 📜 STACK.cpp       # Stack class implementation
├── 📜 demo.cpp        # Demonstration and testing
├── 📜 test.cpp        # Automated tests
├── 📜 log.txt         # Test log output
├── 📜 Makefile        # Build automation
├── 📜 ReadMe.md       # Documentation
```

## Compilation and Execution
This project uses a **Makefile** for easier compilation and execution.

### 1. Build and Run the Demo
```sh
make run_demo
```
This compiles `STACK.cpp` and `demo.cpp`, then runs the demo program.

### 2. Run the Tests
```sh
make run_test
```
This compiles `STACK.cpp` and `test.cpp`, then executes the tests. Results are stored in `log.txt`.

### 3. Clean Compiled Files
```sh
make clean
```
This removes compiled binaries and object files.

## Notes
* The stack operations are **efficient**, running in **O(1) time complexity**.
* The **PImpl idiom** ensures better **encapsulation** and **faster compilation** by reducing header dependencies.
* **Exception handling** prevents illegal stack operations (e.g., popping from an empty stack).
* The **test suite** (`test.cpp`) validates all key functionalities, logging results to `log.txt`.
