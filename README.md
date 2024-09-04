# python_strings

Here’s a complete list of 46 string methods in Python, with explanations and examples:

1. **`capitalize()`**  
   Capitalizes the first character of the string.
   ```python
   s = "hello world"
   print(s.capitalize())  # Output: "Hello world"
   ```

2. **`casefold()`**  
   Converts the string to lowercase, more aggressively than `lower()`.
   ```python
   s = "Hello World"
   print(s.casefold())  # Output: "hello world"
   ```

3. **`center(width, fillchar)`**  
   Centers the string in a field of the specified width, padding with the specified fill character.
   ```python
   s = "hello"
   print(s.center(10, '*'))  # Output: "**hello***"
   ```

4. **`count(substring, start, end)`**  
   Counts the number of occurrences of a substring.
   ```python
   s = "hello world"
   print(s.count('o'))  # Output: 2
   ```

5. **`encode(encoding, errors)`**  
   Encodes the string using the specified encoding.
   ```python
   s = "hello"
   print(s.encode('utf-8'))  # Output: b'hello'
   ```

6. **`endswith(suffix, start, end)`**  
   Checks if the string ends with the specified suffix.
   ```python
   s = "hello world"
   print(s.endswith("world"))  # Output: True
   ```

7. **`expandtabs(tabsize)`**  
   Expands tabs in the string to the specified number of spaces.
   ```python
   s = "hello\tworld"
   print(s.expandtabs(4))  # Output: "hello   world"
   ```

8. **`find(substring, start, end)`**  
   Finds the lowest index where the substring is found, or returns `-1` if not found.
   ```python
   s = "hello world"
   print(s.find("world"))  # Output: 6
   ```

9. **`format(*args, **kwargs)`**  
   Formats the string using the specified arguments.
   ```python
   s = "Hello {}"
   print(s.format("world"))  # Output: "Hello world"
   ```

10. **`format_map(mapping)`**  
    Formats the string using a mapping object.
    ```python
    s = "Hello {name}"
    print(s.format_map({"name": "world"}))  # Output: "Hello world"
    ```

11. **`index(substring, start, end)`**  
    Finds the lowest index where the substring is found, or raises a `ValueError` if not found.
    ```python
    s = "hello world"
    print(s.index("world"))  # Output: 6
    ```

12. **`isalnum()`**  
    Checks if all characters in the string are alphanumeric.
    ```python
    s = "Hello123"
    print(s.isalnum())  # Output: True
    ```

13. **`isalpha()`**  
    Checks if all characters in the string are alphabetic.
    ```python
    s = "Hello"
    print(s.isalpha())  # Output: True
    ```

14. **`isascii()`**  
    Checks if all characters in the string are ASCII.
    ```python
    s = "Hello"
    print(s.isascii())  # Output: True
    ```

15. **`isdecimal()`**  
    Checks if all characters in the string are decimal characters.
    ```python
    s = "123"
    print(s.isdecimal())  # Output: True
    ```

16. **`isdigit()`**  
    Checks if all characters in the string are digits.
    ```python
    s = "123"
    print(s.isdigit())  # Output: True
    ```

17. **`isidentifier()`**  
    Checks if the string is a valid Python identifier.
    ```python
    s = "hello"
    print(s.isidentifier())  # Output: True
    ```

18. **`islower()`**  
    Checks if all characters in the string are lowercase.
    ```python
    s = "hello"
    print(s.islower())  # Output: True
    ```

19. **`isnumeric()`**  
    Checks if all characters in the string are numeric.
    ```python
    s = "123"
    print(s.isnumeric())  # Output: True
    ```

20. **`isprintable()`**  
    Checks if all characters in the string are printable.
    ```python
    s = "hello"
    print(s.isprintable())  # Output: True
    ```

21. **`isspace()`**  
    Checks if the string contains only whitespace characters.
    ```python
    s = "   "
    print(s.isspace())  # Output: True
    ```

22. **`istitle()`**  
    Checks if the string is titlecased (each word starts with an uppercase letter).
    ```python
    s = "Hello World"
    print(s.istitle())  # Output: True
    ```

23. **`isupper()`**  
    Checks if all characters in the string are uppercase.
    ```python
    s = "HELLO"
    print(s.isupper())  # Output: True
    ```

24. **`join(iterable)`**  
    Joins the elements of an iterable (e.g., list) into a string with the string as the separator.
    ```python
    s = "-"
    print(s.join(["hello", "world"]))  # Output: "hello-world"
    ```

25. **`ljust(width, fillchar)`**  
    Left-justifies the string in a field of the specified width, padding with the specified fill character.
    ```python
    s = "hello"
    print(s.ljust(10, '*'))  # Output: "hello*****"
    ```

26. **`lower()`**  
    Converts the string to lowercase.
    ```python
    s = "Hello World"
    print(s.lower())  # Output: "hello world"
    ```

27. **`lstrip(chars)`**  
    Removes leading characters (default is whitespace).
    ```python
    s = "   hello"
    print(s.lstrip())  # Output: "hello"
    ```

28. **`maketrans(x, y, z)`**  
    Returns a translation table used for `translate()`.
    ```python
    table = str.maketrans("abc", "123")
    s = "abc"
    print(s.translate(table))  # Output: "123"
    ```

29. **`partition(separator)`**  
    Splits the string at the first occurrence of the separator into a tuple.
    ```python
    s = "hello world"
    print(s.partition(" "))  # Output: ('hello', ' ', 'world')
    ```

30. **`replace(old, new, count)`**  
    Replaces occurrences of a substring with another substring.
    ```python
    s = "hello world"
    print(s.replace("world", "Python"))  # Output: "hello Python"
    ```

31. **`rfind(substring, start, end)`**  
    Finds the highest index where the substring is found, or returns `-1` if not found.
    ```python
    s = "hello world"
    print(s.rfind("o"))  # Output: 7
    ```

32. **`rindex(substring, start, end)`**  
    Finds the highest index where the substring is found, or raises a `ValueError` if not found.
    ```python
    s = "hello world"
    print(s.rindex("o"))  # Output: 7
    ```

33. **`rjust(width, fillchar)`**  
    Right-justifies the string in a field of the specified width, padding with the specified fill character.
    ```python
    s = "hello"
    print(s.rjust(10, '*'))  # Output: "*****hello"
    ```

34. **`rpartition(separator)`**  
    Splits the string at the last occurrence of the separator into a tuple.
    ```python
    s = "hello world"
    print(s.rpartition(" "))  # Output: ('hello', ' ', 'world')
    ```

35. **`rsplit(separator, maxsplit)`**  
    Splits the string from the right at the separator.
    ```python
    s = "hello world"
    print(s.rsplit(" "))  # Output: ['hello', 'world']
    ```

36. **`rstrip(chars)`**  
    Removes trailing characters (default is whitespace).
    ```python
    s = "hello   "
    print(s.rstrip())  # Output: "hello"
    ```

37. **`split(separator, maxsplit)`**  
    Splits the string at the separator.
    ```python
    s = "hello world"
    print(s.split(" "))  # Output: ['hello', 'world']
    ```

38. **`splitlines(keepends)`**  
    Splits the string at line breaks and returns a list of lines.
    ```python
    s = "hello\nworld"
    print(s.splitlines())  # Output: ['hello', 'world']
    ```

39. **`strip(chars)`**  


    Removes leading and trailing characters (default is whitespace).
    ```python
    s = "   hello   "
    print(s.strip())  # Output: "hello"
    ```

40. **`swapcase()`**  
    Swaps the case of all characters in the string.
    ```python
    s = "Hello World"
    print(s.swapcase())  # Output: "hELLO wORLD"
    ```

41. **`title()`**  
    Capitalizes the first letter of each word.
    ```python
    s = "hello world"
    print(s.title())  # Output: "Hello World"
    ```

42. **`upper()`**  
    Converts the string to uppercase.
    ```python
    s = "Hello World"
    print(s.upper())  # Output: "HELLO WORLD"
    ```

43. **`zfill(width)`**  
    Pads the string on the left with zeros to reach the specified width.
    ```python
    s = "42"
    print(s.zfill(5))  # Output: "00042"
    ```

44. **`lstrip(chars)`**  
    Removes leading characters (default is whitespace).
    ```python
    s = "   hello"
    print(s.lstrip())  # Output: "hello"
    ```

45. **`rfind(substring, start, end)`**  
    Returns the highest index where substring is found or `-1` if not found.
    ```python
    s = "hello world"
    print(s.rfind("o"))  # Output: 7
    ```

46. **`rindex(substring, start, end)`**  
    Returns the highest index where substring is found or raises `ValueError` if not found.
    ```python
    s = "hello world"
    print(s.rindex("o"))  # Output: 7
    ```

Feel free to ask if you need more details or examples for any of these methods!