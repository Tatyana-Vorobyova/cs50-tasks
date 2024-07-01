# CS50’s Introduction to Programming with Python 2022 - Practice Problems Solutions (Lecture 5 - Unit Tests)

This repository contains my solutions to 4 practice problems from the CS50’s Introduction to Programming with Python course. 
Each problem is accompanied by its test file to verify the correctness of the solutions.

## Repository Structure
- bank.py
- test_bank.py
- fuel.py
- test_fuel.py
- plates.py
- test_plates.py
- twttr.py
- test_twttr.py
- README.md

### Files Description

**bank.py**

A program that prompts the user for a greeting. 
If the greeting starts with “hello”, output $0. 
If the greeting starts with an “h” (but not “hello”), output $20. 
Otherwise, output $100.
Ignore any leading whitespace in the user’s greeting, and treat the user’s greeting case-insensitively.

**test_bank.py**

Test cases:
1. A full word "hello" ("hello")
2. Uppercase "hello" and comma ("Hello, David")
3. Letter "h" at the beginning ("hey")
4. Letters different than "h" ("What's up")

**fuel.py**

A program that prompts the user for a fraction, formatted as X/Y, wherein each of X and Y is an integer, and then outputs, as a percentage rounded to the nearest integer, how much fuel is in the tank. 
If, though, 1% or less remains, output E instead to indicate that the tank is essentially empty. And if 99% or more remains, output F instead to indicate that the tank is essentially full.
If, though, X or Y is not an integer, X is greater than Y, or Y is 0, instead prompt the user again. (It is not necessary for Y to be 4.) Catch any exceptions like ValueError or ZeroDivisionError.

**test_fuel.py**

Test cases:
1. A positive convert ("1/4")
2. Division by Zero ("1/0")
3. Value error ("cat/dog")
4. Full tank 99 ("99")
5. Full tank 100 ("100")
6. Empty tank 1 ("1")
7. Empty tank 0 ("0")
8. Medium positive value ("25")

**plates.py**

A program that prompts the user for a vanity plate and then output Valid if meets all of the requirements or Invalid if it does not. 
Assume that any letters in the user’s input will be uppercase. Return True if a plate meets all requirements and False if it does not.

Requirements:
- “All vanity plates must start with at least two letters.”
- “… vanity plates may contain a maximum of 6 characters (letters or numbers) and a minimum of 2 characters.”
- “Numbers cannot be used in the middle of a plate; they must come at the end. For example, AAA222 would be an acceptable … vanity plate; AAA22A would not be acceptable. The first number used cannot be a ‘0’.”
- “No periods, spaces, or punctuation marks are allowed.”

**test_plates.py**

Test cases:
1. A correct plate containing all valid characters ("CS50")
2. Only one letter ("C")
3. Only one number ("50")
4. Maximum valid capacity ("THISIS50")
5. Punctuation mark usage ("AC!.5")
6. Number inside of the letters ("CS50P")
7. Zero placement as the first number ("CS50P")

**twttr.py**

A program that prompts the user for a str of text and then outputs that same text but with all vowels (A, E, I, O, and U) omitted, whether inputted in uppercase or lowercase.

**test_twttr.py**

Test cases:
1. "twitter" string ("twitter")
2. Lowercase string ("abc")
3. Uppercase string ("APPLE")
4. String including numbers ("CS50")
5. String inclusing punctuation ("CS50!")

   

