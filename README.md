# BigInt Library

## Description

The **BigInt Library** is a C++ library that provides a comprehensive implementation for handling large integers beyond the standard data type limits. This library supports various arithmetic operations, comparison operations, and advanced functions such as calculating Fibonacci numbers, Catalan numbers, and factorials of large integers. 

## Features

- **Arithmetic Operations**: Addition, Subtraction, Multiplication, Division, Modulo, and Power functions for large integers.
- **Comparison Operations**: Standard comparison operators (`==`, `!=`, `<`, `>`, `<=`, `>=`).
- **Increment/Decrement**: Pre and Post increment/decrement operators.
- **Advanced Functions**: 
  - Calculation of Fibonacci numbers.
  - Calculation of Catalan numbers.
  - Calculation of Factorials.
  - Square root of large integers.
- **Stream Support**: Input and output stream operators for easy I/O operations.
- **Exception Handling**: Throws exceptions for arithmetic errors like division by zero and underflow.

## Usage

### Basic Usage

```cpp
#include <iostream>
#include "BigInt.h"

int main() {
    BigInt first("12345");
    std::cout << "The number of digits in first big integer = " << numDigits(first) << '\n';

    BigInt second(12345);
    if (first == second) {
        std::cout << "first and second are equal!\n";
    } else {
        std::cout << "Not equal!\n";
    }

    // More operations
}

```

### Advanced Usage

```cpp
#include <iostream>
#include "BigInt.h"

int main() {
    BigInt sum = BigInt("100000") + BigInt("123456789");
    std::cout << "Sum = " << sum << '\n';

    BigInt product = BigInt("98765") * BigInt("4321");
    std::cout << "Product = " << product << '\n';

    BigInt fib = getNthFibonacci(100);
    std::cout << "100th Fibonacci number = " << fib << '\n';

    BigInt catalan = getNthCatalan(20);
    std::cout << "20th Catalan number = " << catalan << '\n';

    BigInt fact = getFactorial(25);
    std::cout << "Factorial of 25 = " << fact << '\n';
}
```

## License
This project is licensed under the MIT License.

## Contributor
Ashmandeep Singh Joshan
