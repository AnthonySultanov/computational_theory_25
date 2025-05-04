# Computational Theory 25

This repository contains tasks and implementations related to computational theory concepts, including:

- Binary operations and their applications in cryptography.
- Hash functions and their translation from C to Python.
- Prime number generation using iterative and sieve methods.
- SHA-256 padding and its implementation.
- Fractional parts of square roots for cryptographic applications.
- Proof of work using SHA-256 hashes of English words.
- Turing machine simulation for binary increment.
- Computational complexity analysis of Bubble Sort.

## Repository Structure

- **tasks.ipynb**: Contains the implementation and explanation of various computational theory tasks.
- **test_sha256.txt**: A sample file used for testing SHA-256 padding.
- **words.txt**: A list of English words used for the proof-of-work task.

## How to Use

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd computational_theory_25
    ```

2. Open `tasks.ipynb` in your preferred Jupyter Notebook environment or Visual Studio Code.

3. Follow the tasks and run the code cells to explore the concepts.

## Tasks Overview

### Task 1: Binary Representations
**Overview**: Explores bitwise operations on 32-bit unsigned integers, including left and right rotations, bitwise choice, and majority functions. These operations are foundational in cryptographic algorithms like SHA-256.

**Key Functions**:
- `rotl(x, n)`: Left rotation.
- `rotr(x, n)`: Right rotation.
- `ch(x, y, z)`: Bitwise choice.
- `maj(x, y, z)`: Bitwise majority.

### Task 2: Hash Functions
**Overview**: Converts a simple C-style hash function into Python. Demonstrates how low-level algorithms can be implemented in Python while preserving their logic.

**Key Function**:
- `hash_func(s)`: Computes a hash value for a string using modular arithmetic.

### Task 3: SHA-256 Padding
**Overview**: Implements the padding process required for the SHA-256 hash algorithm. The function converts input data into a format suitable for hashing by adding padding bits and appending the message length.

**Key Function**:
- `padding_sha256(file_path)`: Reads a file, applies SHA-256 padding, and outputs the padded message.

### Task 4: Prime Numbers
**Overview**: Generates the first 100 prime numbers using two methods: iterative prime checking and the Sieve of Eratosthenes. Compares the performance and accuracy of both methods.

**Key Functions**:
- `prime_iterative(limit)`: Iterative prime generation.
- `prime_sieve_create(max)`: Prime generation using the Sieve of Eratosthenes.

### Task 5: Roots
**Overview**: Calculates the fractional part of the square roots of the first 100 prime numbers and converts them into 32-bit binary integers. This process is used in cryptographic algorithms like SHA-256.

**Key Function**:
- `fractional_32bit(num)`: Extracts the 32-bit fractional part of a square root.

### Task 6: Proof of Work
**Overview**: Simulates a proof of work system by finding English words whose SHA-256 hashes start with the most leading zero bits. This task mimics the concept of blockchain mining.

**Key Functions**:
- `sha256binary(word)`: Computes the SHA-256 hash of a word and converts it to binary.
- `count_leading_zeros(binary_str)`: Counts leading zero bits in a binary string.

### Task 7: Turing Machines
**Overview**: Simulates a Turing machine that performs binary increment. Demonstrates how simple rules can drive a machine through states to process input on a tape.

**Key Function**:
- `turingmachine(tape)`: Simulates a Turing machine with a given input tape.

### Task 8: Computational Complexity
**Overview**: Analyzes the computational complexity of Bubble Sort by counting the number of comparisons required to sort all permutations of a list. Demonstrates best-case, worst-case, and average-case scenarios.

**Key Function**:
- `bubble_sort_with_comparisons`: Sorts a list using Bubble Sort and counts the number of comparisons.

## Installation

1. Clone the Repository:
    ```bash
    git clone <repository-url>
    cd computational_theory_25
    ```

2. Install Dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Notebook:
    Open `tasks.ipynb` in Jupyter Notebook and execute the cells.

## Dependencies

- **Python 3.x**
- **Libraries**:
  - `matplotlib`: For visualizations.
  - `nltk`: For verifying English words in Task 6.
  - Built-in libraries: `hashlib`, `math`, `itertools`.

## References by Task

- **Task 1: Binary Representations**
  - [Python Bitwise Operators – Official Docs](https://docs.python.org/3/library/stdtypes.html#bitwise-operations)
  - GeeksforGeeks: Bitwise Operators in Python
- **Task 2: Hash Functions**
  - Kernighan, B. W., & Ritchie, D. M. (1988). *The C Programming Language*.
- **Task 3: SHA-256 Padding**
  - FIPS PUB 180-4: Secure Hash Standard
  - Wikipedia: SHA-2
- **Task 4: Prime Numbers**
  - Sieve of Eratosthenes – Wikipedia
- **Task 5: Roots**
  - Square Root – Wikipedia
- **Task 6: Proof of Work**
  - SHA-256 – Wikipedia
  - Proof of Work – Bitcoin Wiki
- **Task 7: Turing Machines**
  - Turing, A. M. (1937). *On Computable Numbers*.
- **Task 8: Computational Complexity**
  - GeeksforGeeks: Bubble Sort
  - Cormen, T. H., et al. (2009). *Introduction to Algorithms*.