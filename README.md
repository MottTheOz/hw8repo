Ryan Mott
UMBC / CMSC 313,
May 18, 2025 - I am aware this is a late submission and apologize for it.

This project implements a matrix manipulation library in both C and C++. The libraries provide functionalities for matrix creation, deallocation, printing, scalar multiplication, matrix addition, matrix transpose, and matrix on matrix multiplication.

Its goal is to show these operations by calculating the matrix expression $D = A + (3 \times B) \times C^T$, where A, B, and C are already defined matrices.

## FILES

* `README.md`: This document provides overview and instructions for the project.
* `Makefile`: Streamlines the commands for both the C and C++ compilation processes

### C Version (`c_version/`)
* `c_version/matrix.h`: Header file for the C matrix library. Defines the `Matrix` struct and declares the matrix manipulation functions.
* `c_version/matrix.c`: Implementation file for the C matrix library. Contains the definitions of the functions declared in `matrix.h`.
* `c_version/main_c.c`: The main test program for the C matrix library. It initializes matrices A, B, and C, performs the required calculation $D = A + (3B)C^T$, and prints the resulting matrix D.

### C++ Version (`cpp_version/`)
* `cpp_version/Matrix.hpp`: Header file for the C++ `Matrix` class. Defines the class interface, including constructors, destructors (if necessary), operator overloads, and member functions.
* `cpp_version/Matrix.cpp`: Implementation file for the C++ `Matrix` class. Contains the definitions of the methods and overloaded operators declared in `Matrix.hpp`.
* `cpp_version/main_cpp.cpp`: The main test program for the C++ `Matrix` class. It initializes Matrix objects for A, B, and C, performs the required calculation $D = A + (3B)C^T$ using overloaded operators, and prints the resulting Matrix D.

## GETTING STARTED and RUNNING
## FILES ARE CONTAINED WITHIN A ZIP FOLDER, PLEASE BE SURE TO EXTRACT FIRST (so all of the files can remain within their initial directories for convienience)

**1. Compile both versions:**
* To build both C and C++ versions:
    ```bash
    make all
    ```


**2. Run a specific persion:**
* To run the C version use this command in the main file directory (same one as the makefile):
    ```bash
    ./c_version/c_matrix_test
    ```
* To run the C++ version use this command in the main file directory (same one as the makefile):
    ```bash
    ./cpp_version/cpp_matrix_test
    ```
