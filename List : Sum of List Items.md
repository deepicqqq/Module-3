## NAME: DEEPIKA P
## REGISTER NO: 212223240024
# List Operations in Python: Sum of List Items

## 🎯 Aim
To write a Python program that creates a list with a size and elements entered by the user, using eval() to convert the input strings into appropriate Python data types.

## 🧠 Algorithm
1. Take an integer input from the user representing the size of the list, say n.

2. Initialize an empty list called user_list.

3. Run a loop from 0 to n-1:

4. For each iteration, take input from the user as a string.

5. Use eval() on the input string to convert it to its respective Python data type.

6.Append the evaluated input to user_list.

After the loop ends, print the final list.
## 🧾 Program

def create_list():\
    size = int(input())\
    lst = []

    for _ in range(size):
        element = eval(input())
        lst.append(element)

    print(lst)  # Print the final list

# Example usage:
create_list()


## Output
![Screenshot 2025-05-18 193118](https://github.com/user-attachments/assets/8d0b3623-8847-45ce-8cb9-aaf162a43aad)

## Result
The Python program successfully created a list of specified size with elements of varying types entered by the user, using eval() to parse each input correctly.


# Regex in Python: Filter Words Without the Letter 'e'

## 🎯 Aim
To write a Python program that filters out and returns all elements from a list **that do not contain the letter `'e'`**, using **regular expressions (regex)**.

## 🧠 Algorithm
1. Import the `re` module.
2. Initialize an empty list `l1` to store results.
3. Define a list of words:  
   `items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']`
4. Iterate through each word in the list:
   - Use `re.search(r"e", i)` to check if the word contains `'e'`.
   - If **not**, append the word to `l1`.
5. Print the final filtered list.

## 🧾 Program
import re\
items = ['goal', 'new', 'user', 'sit', 'eat', 'dinner']\
l1 = []

for i in items:\
    if not re.search(r"e", i):\
        l1.append(i)

print("Words without the letter 'e':", l1)

## Output
![Screenshot 2025-05-18 200854](https://github.com/user-attachments/assets/fbbb0107-214b-4dc6-b890-d0f5104f1eb0)

## Result
The program successfully filtered and returned all words from the list that do not contain the letter 'e' using regular expressions.

# Module-3
# 🧹 Strings-Remove Nth Index Character from a String

## 🎯 Aim
To write a Python function named remove that accepts a string and removes all vowels (a, e, i, o, u, both uppercase and lowercase) from it.



## 🧠 Algorithm
1. Define the function remove(s) that takes a string s as input.

2. Initialize an empty string result.

3. Loop through each character in the input string s.

4. If the character is not a vowel (check using not in "aeiouAEIOU"), add it to result.

5. After the loop, return or print the result string.


## 💻 Program
def remove(s):\
    vowels = "aeiouAEIOU"\
    res = "".join(char for char in s if char not in vowels)\
    print(res)

## Output
![Screenshot 2025-05-18 201139](https://github.com/user-attachments/assets/9bde50a2-7764-48aa-91a1-ea3c2ad3a9b1)

## Result
The function remove() correctly removed all vowels from the input string "learning python" and returned the result "lrnng pythn".

# Strings-Palindrome Check in Python (Without Built-in Functions)

## 🎯 Aim
To write a Python program to check whether a string is a palindrome without using built-in string functions.
## 🧠 Algorithm
1. Assign the input string to a variable s.

2. Initialize a variable rev = "" to store the reversed string.

3. Use a for loop to reverse the string manually (iterate from the last character to the first).

4. Compare the reversed string with the original.

5. If both are equal, print that the string is a palindrome.

6. Otherwise, print that it's not a palindrome.

## 🧾 Program
def ispalindrome(a):\
    return a==a[::-1]\
a=input()\
ans=ispalindrome(a)\
if ans:\
    print("The entered string is palindrome")\
else:\
    print("The entered string is not palindrome")

## Output
![Screenshot 2025-05-18 201833](https://github.com/user-attachments/assets/a1011ecc-b5fd-4ca2-abc4-b5e13f39854c)

## Result
The program successfully checks whether the entered string is a palindrome without using built-in functions.


# Tuple in Python: Check Element Existence

## 🎯 Aim
To write a Python program that joins tuples from a list if they share the same initial (first) element.

## 🧠 Algorithm
1. Initialize a tuple of tuples (input data).

2. Create an empty dictionary to group tuples by their first element.

3. Loop through each tuple in the input:

4. Use the first element as the key.

5. Append the second element to the list of values for that key.

6. After grouping, convert each dictionary entry into a new tuple.

7. Store and print the final list of grouped tuples.

## 🧾 Program
n=eval(input())\
print("Initially the tuple is :",n)\
t=[]\
for i in n:\
    if t and t[-1][0]==i[0]:\
        t[-1]+=i[1:]\
    else:\
        t.append(i)\
print("Joined tuple :",tuple(t))


## Output
![Screenshot 2025-05-18 202248](https://github.com/user-attachments/assets/3880a602-b68a-4bc6-9619-93b168933609)

## Result
The program successfully joins tuples that have the same starting element, as required.


