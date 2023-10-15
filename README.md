# change-characterc-
The provided C++ code defines a program that takes a string as input and changes each character in the string to the next character in the alphabet. If the character is 'z', it wraps around to 'a', and if the character is 'Z', it wraps around to 'A'. Other characters that are not alphabetic characters remain unchanged.

Here's a step-by-step explanation of what the code does:

1. It includes necessary headers: `<iostream>` and `<string>` for input/output and string manipulation.

2. The `change_letter` function takes a string `str` as input and returns a modified string with characters changed according to the rules described above.

3. It uses a `for` loop to iterate through each character of the input string.

4. It converts the character to its ASCII code using the `int(str[x])` function and stores it in the `char_code` variable.

5. It checks if `char_code` is equal to 122 (which is 'z' in ASCII) and replaces it with 'a' by assigning the ASCII code of 'a' (97) to `str[x]`.

6. It checks if `char_code` is equal to 90 (which is 'Z' in ASCII) and replaces it with 'A' by assigning the ASCII code of 'A' (65) to `str[x]`.

7. It checks if `char_code` is within the range of uppercase and lowercase alphabetic characters (i.e., between 'A' and 'Z' or between 'a' and 'z'). If so, it increments `char_code` by 1 and assigns the corresponding character to `str[x]`.

8. The modified string is returned.

9. In the `main` function, two strings are provided as input to the `change_letter` function: "Ouassim". The original strings are printed, and then the modified strings are printed.

However, there is a minor issue in the code. The original string is printed twice in the `main` function. It might be a copy-paste error, and you may want to remove the duplicate lines:

```cpp
int main() {
    cout << "Original string: Ouassim"; 
    cout << "\nNew string: " << change_letter("Ouassim");
    return 0;
}
```

With this change, the code should work as expected, converting the original string "Ouassim" to the next characters in the alphabet and printing the original and modified strings once.
