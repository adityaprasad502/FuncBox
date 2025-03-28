# FuncBox

FuncBox is a versatile Python utility library designed to provide a wide range of common operations and aims to simplify everyday programming tasks by offering easy-to-use functions.


## Installation

To install FuncBox, use pip:

```bash
pip install -U funcbox
```

## Usage

Import FuncBox into your Python project to access its functions:

```python
from funcbox import *
```

## Available Functions

FuncBox is organized into categories for easy navigation:

### Mathematical Operations

*   **`is_even(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is even.
    - **Parameters**:
        - `number`: An integer or a list of integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is even, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer or a list of integers.
    - **Examples**:
        ```python
        print(is_even(4))  # Output: True
        print(is_even([3, 4, 7]))  # Output: [False, True, False]
        ```

*   **`is_odd(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is odd.
    - **Parameters**:
        - `number`: An integer or a list of integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is odd, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer or a list of integers.
    - **Examples**:
        ```python
        print(is_odd(5))  # Output: True
        print(is_odd([2, 5, 8]))  # Output: [False, True, False]
        ```

*   **`factorial(number: Union[int, List[int]]) -> Union[int, List[int]]`**:
    Computes the factorial of a given number or a list of numbers.
    - **Parameters**:
        - `number`: A non-negative integer or a list of non-negative integers.
    - **Returns**:
        - `int` or `List[int]`: The factorial of the number. Returns a list of factorials if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is negative, or is not a list of integers.
    - **Examples**:
        ```python
        print(factorial(5))  # Output: 120
        print(factorial([3, 4]))  # Output: [6, 24]
        ```

*   **`is_prime(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is prime.
    - **Parameters**:
        - `number`: A non-negative integer or a list of non-negative integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is prime, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is negative, or is not a list of integers.
    - **Examples**:
        ```python
        print(is_prime(11))  # Output: True
        print(is_prime([4, 7, 9]))  # Output: [False, True, False]
        ```

*   **`fibonacci(number: Union[int, List[int]]) -> Union[int, List[int]]`**:
    Computes the Fibonacci number for a given non-negative integer or a list of non-negative integers.
    - **Parameters**:
        - `number`: A non-negative integer or a list of non-negative integers.
    - **Returns**:
        - `int` or `List[int]`: The Fibonacci number. Returns a list of Fibonacci numbers if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is negative, or is not a list of integers.
    - **Examples**:
        ```python
        print(fibonacci(6))  # Output: 8
        print(fibonacci([7, 8]))  # Output: [13, 21]
        ```

*   **`is_armstrong(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is an Armstrong number.
    - **Parameters**:
        - `number`: A non-negative integer or a list of non-negative integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is an Armstrong number, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is negative, or is not a list of integers.
    - **Examples**:
        ```python
        print(is_armstrong(153))  # Output: True
        print(is_armstrong([370, 9474]))  # Output: [True, True]
        ```

*   **`is_perfect(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is a perfect number.
    - **Parameters**:
        - `number`: A positive integer or a list of positive integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is a perfect number, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is not positive, or is not a list of integers.
    - **Examples**:
        ```python
        print(is_perfect(6))  # Output: True
        print(is_perfect([28, 496]))  # Output: [True, True]
        ```

*   **`is_harshad(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is a Harshad number (divisible by the sum of its digits).
    - **Parameters**:
        - `number`: A positive integer or a list of positive integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is a Harshad number, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is not positive, or is not a list of integers.
    - **Examples**:
        ```python
        print(is_harshad(18))  # Output: True
        print(is_harshad([21, 27]))  # Output: [True, True]
        ```

*   **`is_disarium(number: Union[int, List[int]]) -> Union[bool, List[bool]]`**:
    Checks if a given number or a list of numbers is a Disarium number (sum of digits raised to their respective positions equals the number).
    - **Parameters**:
        - `number`: A positive integer or a list of positive integers to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the number is a Disarium number, `False` otherwise. Returns a list of boolean values if a list of numbers is provided.
    - **Raises**:
        - `ValueError`: If the input is not an integer, is not positive, or is not a list of integers.
    - **Examples**:
        ```python
        print(is_disarium(175))  # Output: True
        print(is_disarium([518, 598]))  # Output: [True, True]
        ```

*   **`average(*args: float) -> float`**:
    Calculates the average of a list of numbers.
    - **Parameters**:
        - `*args`: Variable number of numerical arguments (integers or floats).
    - **Returns**:
        - `float`: The average of the input numbers. Returns 0.0 if no arguments are provided.
    - **Raises**:
        - `ValueError`: If any of the arguments are not numbers.
    - **Examples**:
        ```python
        print(average(1, 2, 3, 4, 5))  # Output: 3.0
        ```

*   **`percentage(part: float, whole: float) -> float`**:
    Calculates the percentage of a part in relation to a whole.
    - **Parameters**:
        - `part`: The part value (integer or float).
        - `whole`: The whole value (integer or float).
    - **Returns**:
        - `float`: The percentage value.
    - **Raises**:
        - `ValueError`: If `part` or `whole` are not numbers, or if `whole` is zero.
    - **Examples**:
        ```python
        print(percentage(20, 100))  # Output: 20.0
        ```

*   **`percentile(data: List[float], n: float) -> float`**:
    Calculates the nth percentile of a list of numbers.
    - **Parameters**:
        - `data`: A list of numbers (integers or floats).
        - `n`: The percentile to calculate (a number between 0 and 100).
    - **Returns**:
        - `float`: The nth percentile value.
    - **Raises**:
        - `ValueError`: If `data` is not a list of numbers, or if `n` is not a number between 0 and 100.
    - **Examples**:
        ```python
        print(percentile([1, 2, 3, 4, 5], 50))  # Output: 3.0
        ```

*   **`gcd(a: int, b: int) -> int`**:
    Calculates the greatest common divisor of two numbers.
    - **Parameters**:
        - `a`: The first integer.
        - `b`: The second integer.
    - **Returns**:
        - `int`: The greatest common divisor of `a` and `b`.
    - **Raises**:
        - `ValueError`: If `a` or `b` are not integers.
    - **Examples**:
        ```python
        print(gcd(12, 18))  # Output: 6
        ```

*   **`lcm(a: int, b: int) -> int`**:
    Calculates the least common multiple of two numbers.
    - **Parameters**:
        - `a`: The first integer.
        - `b`: The second integer.
    - **Returns**:
        - `int`: The least common multiple of `a` and `b`.
    - **Raises**:
        - `ValueError`: If `a` or `b` are not integers.
    - **Examples**:
        ```python
        print(lcm(12, 18))  # Output: 36
        ```

*   **`dijkstra(graph: dict, start_node: Any) -> dict`**:
    Compute Dijkstra’s shortest path algorithm to find the shortest paths from a start node to all other nodes in a graph.
    - **Parameters**:
        - `graph`: A graph represented as an adjacency list, where keys are nodes and values are dictionaries mapping neighbors to edge weights.
        - `start_node`: The node to start the pathfinding from.
    - **Returns**:
        - `dict`: A dictionary containing two dictionaries:
              - `'distances'`: Shortest distances from the start node to each node.
              - `'paths'`: Shortest paths from the start node to each node.
              Nodes not reachable from the start node will have a distance of infinity and path as None.
    - **Raises**:
        - `ValueError`: If the graph is not a dictionary or the `start_node` is not in the graph.
    - **Examples**:
        ```python
        graph = {
            'A': {'B': 4, 'C': 2},
            'B': {'D': 5, 'E': 1},
            'C': {'B': 1, 'E': 3},
            'D': {'F': 2},
            'E': {'D': 1, 'F': 4},
            'F': {}
        }
        result = dijkstra(graph, 'A')
        print(result['distances'])
        # Output: {'A': 0, 'B': 3, 'C': 2, 'D': 4, 'E': 4, 'F': 6}
        print(result['paths'])
        # Output: {'A': ['A'], 'B': ['A', 'C', 'B'], 'C': ['A', 'C'], 'D': ['A', 'C', 'B', 'E', 'D'], 'E': ['A', 'C', 'E'], 'F': ['A', 'C', 'B', 'E', 'D', 'F']}
        ```

### String Operations

*   **`is_palindrome(string: Union[str, List[str]]) -> Union[bool, List[bool]]`**:
    Checks if a given string or a list of strings is a palindrome.
    - **Parameters**:
        - `string`: A string or a list of strings to be checked.
    - **Returns**:
        - `bool` or `List[bool]`: `True` if the string is a palindrome, `False` otherwise. Returns a list of boolean values if a list of strings is provided.
    - **Raises**:
        - `ValueError`: If the input is not a string, is an empty string, or is not a list of strings.
    - **Examples**:
        ```python
        print(is_palindrome("racecar"))  # Output: True
        print(is_palindrome(["hello", "madam"]))  # Output: [False, True]
        ```

*   **`camel_to_snake(name: str) -> str`**:
    Converts a string from camel case to snake case.
    - **Parameters**:
        - `name`: The string in camel case to be converted.
    - **Returns**:
        - `str`: The converted string in snake case.
    - **Raises**:
        - `ValueError`: If the input is not a string.
    - **Examples**:
        ```python
        print(camel_to_snake("camelCaseText"))  # Output: camel_case_text
        ```

*   **`snake_to_camel(name: str) -> str`**:
    Converts a string from snake case to camel case.
    - **Parameters**:
        - `name`: The string in snake case to be converted.
    - **Returns**:
        - `str`: The converted string in camel case.
    - **Raises**:
        - `ValueError`: If the input is not a string.
    - **Examples**:
        ```python
        print(snake_to_camel("snake_case_text"))  # Output: SnakeCaseText
        ```

*   **`slugify(text: str) -> str`**:
    Converts a string into a URL-friendly slug by removing non-alphanumeric characters, stripping whitespace, and replacing spaces with hyphens.
    - **Parameters**:
        - `text`: The string to be slugified.
    - **Returns**:
        - `str`: The slugified string.
    - **Raises**:
        - `ValueError`: If the input is not a string.
    - **Examples**:
        ```python
        print(slugify("This is a test string"))  # Output: this-is-a-test-string
        ```

*   **`count_words(text: str) -> int`**:
    Counts the number of words in a given text.
    - **Parameters**:
        - `text`: The string to count words from.
    - **Returns**:
        - `int`: The number of words in the text.
    - **Raises**:
        - `ValueError`: If the input is not a string.
    - **Examples**:
        ```python
        print(count_words("This is a sentence.")) # Output: 4
        ```

*   **`get_word_count(text: str) -> dict`**:
    Counts the occurrences of each word in a text and returns a dictionary.
    - **Parameters**:
        - `text`: The string to analyze.
    - **Returns**:
        - `dict`: A dictionary where keys are words and values are their counts.
    - **Raises**:
        - `ValueError`: If the input is not a string.
    - **Examples**:
        ```python
        print(get_word_count("This is is a sentence.")) # Output: {'this': 1, 'is': 2, 'a': 1, 'sentence': 1}
        ```

*   **`get_char_count(text: str) -> dict`**:
    Counts the occurrences of each character in a text and returns a dictionary.
    - **Parameters**:
        - `text`: The string to analyze.
    - **Returns**:
        - `dict`: A dictionary where keys are characters and values are their counts.
    - **Raises**:
        - `ValueError`: If the input is not a string.
    - **Examples**:
        ```python
        print(get_char_count("hello")) # Output: {'h': 1, 'e': 1, 'l': 2, 'o': 1}
        ```

*   **`fuzzy_search(search_term: str, text_list: List[str]) -> Union[str, None]`**:
    Fuzzy searches for the best match of a search term within a list of strings.
    - **Parameters**:
        - `search_term`: The string to search for.
        - `text_list`: A list of strings to search within.
    - **Returns**:
        - `Union[str, None]`: The best matching string from the list or `None` if no good match is found (score less than 60).
    - **Examples**:
        ```python
        strings = ["apple", "banana", "cherry", "date"]
        print(fuzzy_search("appel", strings))  # Output: apple
        print(fuzzy_search("bananas", strings)) # Output: banana
        print(fuzzy_search("grape", strings))  # Output: None
        ```

### Location Operations

*   **`calculate_distance(coord1: tuple, coord2: tuple) -> float`**:
    Calculate the distance between two geographical coordinates using the Haversine formula.
    - **Parameters**:
        - `coord1`: Tuple of (latitude, longitude) for the first coordinate in degrees.
        - `coord2`: Tuple of (latitude, longitude) for the second coordinate in degrees.
    - **Returns**:
        - `float`: The distance between the two coordinates in centimeters.
    - **Raises**:
        - `ValueError`: If the input coordinates are not tuples of length 2, or if latitude/longitude values are not floats.
    - **Examples**:
        ```python
        print(calculate_distance((40.7128, -74.0060), (34.0522, -118.2437)))
        # Output: 393574394.19
        ```

### Time Operations

*   **`time_ago(timestamp: datetime, detailed: bool = True, short: bool = False) -> str`**:
    Calculates and returns a human-readable string representing the time elapsed since a given datetime object.
    - **Parameters**:
        - `timestamp`: A datetime object representing the past time.
        - `detailed`: (Optional) If `True` (default), returns a detailed time ago string. If `False`, returns a less detailed string (e.g., only the largest unit of time).
        - `short`: (Optional) If `True`, returns a short format (e.g., "5m" for 5 minutes).
    - **Returns**:
        - `str`: A string indicating how long ago the timestamp was (e.g., "5 minutes ago", "just now").
    - **Raises**:
        - `ValueError`: If the input timestamp is not a datetime object.
    - **Examples**:
        ```python
        from datetime import datetime, timedelta
        now = datetime.now()
        past_time = now - timedelta(minutes=5)
        print(time_ago(past_time))          # Output: 5 minutes ago
        print(time_ago(past_time, short=True)) # Output: 5m ago
        ```

*   **`get_current_date(format_str: str = '%Y-%m-%d') -> str`**:
    Retrieves the current date and formats it as a string according to the specified format.
    - **Parameters**:
        - `format_str`: (Optional) A string specifying the desired date format (default is '%Y-%m-%d'). Uses standard Python datetime format codes.
    - **Returns**:
        - `str`: The current date as a formatted string.
    - **Raises**:
        - `ValueError`: If the input `format_str` is not a string.
    - **Examples**:
        ```python
        print(get_current_date())         # Output: (e.g., "2025-03-08")
        print(get_current_date('%d/%m/%Y')) # Output: (e.g., "08/03/2025")
        ```

*   **`get_current_time(format_str: str = '%H:%M:%S') -> str`**:
    Retrieves the current time and formats it as a string according to the specified format.
    - **Parameters**:
        - `format_str`: (Optional) A string specifying the desired time format (default is '%H:%M:%S'). Uses standard Python datetime format codes.
    - **Returns**:
        - `str`: The current time as a formatted string.
    - **Raises**:
        - `ValueError`: If the input `format_str` is not a string.
    - **Examples**:
        ```python
        print(get_current_time())         # Output: (e.g., "15:30:45")
        print(get_current_time('%I:%M %p')) # Output: (e.g., "03:30 PM")
        ```

*   **`get_day_of_week() -> str`**:
    Returns the current day of the week as a string (e.g., "Monday", "Tuesday").
    - **Returns**:
        - `str`: The current day of the week.
    - **Examples**:
        ```python
        print(get_day_of_week()) # Output: (e.g., "Saturday")
        ```

*   **`calculate_age(birth_date: str, date_format: str = '%Y-%m-%d') -> int`**:
    Calculates the age in years based on a birth date provided as a string.
    - **Parameters**:
        - `birth_date`: A string representing the birth date.
        - `date_format`: (Optional) The format of the birth date string (default is '%Y-%m-%d').
    - **Returns**:
        - `int`: The calculated age in years.
    - **Raises**:
        - `ValueError`: If `birth_date` or `date_format` is not a string, or if the `birth_date` string does not match the `date_format`.
    - **Examples**:
        ```python
        print(calculate_age('1990-05-15')) # Output: (e.g., 34)
        print(calculate_age('15/05/1990', '%d/%m/%Y')) # Output: (e.g., 34)
        ```

### Statistical Operations

*   **`mean_val(numbers: List[Union[int, float]]) -> float`**:
    Calculates the arithmetic mean (average) of a list of numbers.
    - **Parameters**:
        - `numbers`: A list of numbers (integers or floats).
    - **Returns**:
        - `float`: The mean value of the numbers. Returns 0.0 for an empty list.
    - **Raises**:
        - `ValueError`: If the input is not a list.
    - **Examples**:
        ```python
        print(mean_val([1, 2, 3, 4, 5]))  # Output: 3.0
        ```

*   **`median_val(numbers: List[Union[int, float]]) -> float`**:
    Calculates the median value of a list of numbers.
    - **Parameters**:
        - `numbers`: A list of numbers (integers or floats).
    - **Returns**:
        - `float`: The median value of the numbers. Returns 0.0 for an empty list.
    - **Raises**:
        - `ValueError`: If the input is not a list.
    - **Examples**:
        ```python
        print(median_val([1, 2, 3, 4, 5]))  # Output: 3.0
        print(median_val([1, 2, 3, 4]))  # Output: 2.5
        ```

*   **`mode_val(numbers: List[Union[int, float]]) -> List[Union[int, float]]`**:
    Calculates the mode(s) of a list of numbers. The mode is the value that appears most frequently.
    - **Parameters**:
        - `numbers`: A list of numbers (integers or floats).
    - **Returns**:
        - `List[Union[int, float]]`: A list of mode values. Returns an empty list if the input list is empty. If there are multiple modes (values with the same highest frequency), all modes are returned.
    - **Raises**:
        - `ValueError`: If the input is not a list.
    - **Examples**:
        ```python
        print(mode_val([1, 2, 2, 3, 3, 3]))  # Output: [3]
        print(mode_val([1, 2, 2, 3, 3]))  # Output: [2, 3]
        ```

### Unit Conversion Operations

*   **`convert_to_celsius(fahrenheit: float) -> float`**:
    Converts a temperature from Fahrenheit to Celsius.
    - **Parameters**:
        - `fahrenheit`: Temperature in Fahrenheit.
    - **Returns**:
        - `float`: Temperature in Celsius.
    - **Raises**:
        - `ValueError`: If the input is not a number (int or float).
    - **Examples**:
        ```python
        print(convert_to_celsius(68)) # Output: 20.0
        ```

*   **`convert_to_fahrenheit(celsius: float) -> float`**:
    Converts a temperature from Celsius to Fahrenheit.
    - **Parameters**:
        - `celsius`: Temperature in Celsius.
    - **Returns**:
        - `float`: Temperature in Fahrenheit.
    - **Raises**:
        - `ValueError`: If the input is not a number (int or float).
    - **Examples**:
        ```python
        print(convert_to_fahrenheit(20)) # Output: 68.0
        ```

*   **`kg_to_lbs(kg: float) -> float`**:
    Converts weight from kilograms to pounds.
    - **Parameters**:
        - `kg`: Weight in kilograms.
    - **Returns**:
        - `float`: Weight in pounds.
    - **Raises**:
        - `ValueError`: If the input is not a number (int or float).
    - **Examples**:
        ```python
        print(kg_to_lbs(10)) # Output: 22.0462
        ```

*   **`lbs_to_kg(lbs: float) -> float`**:
    Converts weight from pounds to kilograms.
    - **Parameters**:
        - `lbs`: Weight in pounds.
    - **Returns**:
        - `float`: Weight in kilograms.
    - **Raises**:
        - `ValueError`: If the input is not a number (int or float).
    - **Examples**:
        ```python
        print(lbs_to_kg(22.0462)) # Output: 10.0
        ```

*   **`miles_to_km(miles: float) -> float`**:
    Converts distance from miles to kilometers.
    - **Parameters**:
        - `miles`: Distance in miles.
    - **Returns**:
        - `float`: Distance in kilometers.
    - **Raises**:
        - `ValueError`: If the input is not a number (int or float).
    - **Examples**:
        ```python
        print(miles_to_km(10)) # Output: 16.0934
        ```

*   **`km_to_miles(km: float) -> float`**:
    Converts distance from kilometers to miles.
    - **Parameters**:
        - `km`: Distance in kilometers.
    - **Returns**:
        - `float`: Distance in miles.
    - **Raises**:
        - `ValueError`: If the input is not a number (int or float).
    - **Examples**:
        ```python
        print(km_to_miles(16.0934)) # Output: 10.0
        ```

## Disclaimer

FuncBox provides utility functions for general use. The developer is not responsible for any issues caused by improper use or abuse of the library.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request with your improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
