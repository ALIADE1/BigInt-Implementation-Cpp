# BigInt-CPP

A C++ implementation of a `BigInt` class for handling large integers, supporting addition, exponentiation, and increment operations.

## Features

- **Big Integer Addition** (`+` operator overload)
- **Exponentiation** (`^` operator using `std::pow`)
- **Increment Operator** (`++` postfix overload)
- **String and Integer Constructors**
- **Friend Functions for Mixed-Type Addition**
- **Custom Destructor for Debugging**

## Files Structure

- `BigInt.h` – Contains the `BigInt` class definition and operator overloads.
- `Code.cpp` – Example usage of `BigInt` with tests.

## Usage

### 1. Include the header file:
```cpp
#include "BigInt.h"
```

### 2. Creating `BigInt` objects
```cpp
BigInt a("123456789");
BigInt b(98765);
BigInt c = "314159";
```

### 3. Performing Addition
```cpp
BigInt sum = a + b;
cout << "Sum: " << sum << endl;
```

### 4. Exponentiation
```cpp
BigInt base(2);
BigInt exponent(10);
BigInt power = base ^ exponent;
cout << "Power: " << power << endl; // Output: 1024
```

### 5. Postfix Increment (`i++`)
```cpp
BigInt i = 15;
i++;
cout << "After Increment: " << i << endl;
```

## Compilation
Compile using a C++ compiler such as `g++`:
```sh
g++ Code.cpp -o big_int_test -std=c++11
./big_int_test
```

## Notes
- The exponentiation function converts `BigInt` values to `long long`, limiting its range to 64-bit integers.
- The destructor outputs "Dying" when an object is destroyed.

## License
This project is open-source. Feel free to use and modify it!

