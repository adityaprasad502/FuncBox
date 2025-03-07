# FuncBox

FuncBox is a Python package that provides a set of useful utility functions for common mathematical and string operations.

## Installation

You can install FuncBox using pip:

```bash
pip install -U funcbox
```

## Usage

After installing the package, you can import and use the functions as follows:

```python
from funcbox import *

# Check if a single number is even or a list of numbers are even
print(is_even(4))  # Output: True
print(is_even(5))  # Output: False
print(is_even([4, 5, 6]))  # Output: [True, False, True]

# Check if a single number is odd or a list of numbers are odd
print(is_odd(4))  # Output: False
print(is_odd(5))  # Output: True
print(is_odd([4, 5, 6]))  # Output: [False, True, False]

# Compute factorial of a single number or a list of numbers
print(factorial(5))  # Output: 120
print(fact(5))  # Output: 120 (fact is an alias for factorial)
print(factorial([3, 4, 5]))  # Output: [6, 24, 120]

# Check if a single number is prime or a list of numbers are prime
print(is_prime(11))  # Output: True
print(is_prime(4))  # Output: False
print(is_prime([11, 4, 7]))  # Output: [True, False, True]

# Check if a single string is a palindrome or a list of strings are palindromes
print(is_palindrome("racecar"))  # Output: True
print(is_palindrome("hello"))  # Output: False
print(is_palindrome(["racecar", "hello", "madam"]))  # Output: [True, False, True]

# Check if a single number is an Armstrong number or a list of numbers are Armstrong numbers
print(is_armstrong(153))  # Output: True
print(is_armstrong(123))  # Output: False
print(is_armstrong([153, 123, 370]))  # Output: [True, False, True]
```

## Available Functions

### `is_even(number: Union[int, List[int]]) -> Union[bool, List[bool]]`
Checks if a given integer or a list of integers is even.

### `is_odd(number: Union[int, List[int]]) -> Union[bool, List[bool]]`
Checks if a given integer or a list of integers is odd.

### `factorial(number: Union[int, List[int]]) -> Union[int, List[int]]`
Computes the factorial of a given non-negative integer or a list of non-negative integers. An alias `fact` is also available for this function.

### `is_prime(number: Union[int, List[int]]) -> Union[bool, List[bool]]`
Checks if a given positive integer or a list of positive integers is prime.

### `is_palindrome(string: Union[str, List[str]]) -> Union[bool, List[bool]]`
Checks if a given string or a list of strings is a palindrome (ignoring spaces and case).

### `is_armstrong(number: Union[int, List[int]]) -> Union[bool, List[bool]]`
Checks if a given positive integer or a list of positive integers is an Armstrong number.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
