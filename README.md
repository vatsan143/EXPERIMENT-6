# EXPERIMENT-6
## AIM:To write a Python program for checking Palindrome and to write test cases for ir. 

## ALGORITHM
Step 1: Start
Step 2: Get an input from the user by prompting
Step 3: Run a loop form 0 to len/2.
Step 4: Check if the characters are the same both from the start and the end till len/2.
Step 5: If it is, return the result that it is a palindrome.
Step 6: Else, return that it is not a palindrome.
Step 7: Stop. 

## PROGRAM
### NAME: SRIVATSAN G

### REG NO: 212223230216
```
def Palindrome(string):
    for i in range(0, int(len(string) / 2)):
        if string[i] != string[len(string) - i - 1]:  # Fixed indexing
            return False
    return True


s = input("Enter a string: ")  # Added a prompt for clarity

c = 1
for i in s:
    if not i.isalpha():
        c = 0
        break  # Added break to stop checking after finding a non-alphabetic character

if c == 0:
    print("Enter a valid string")
    print("Test Case:Fail")
else:
    answer = Palindrome(s)
    if answer:
        print("The given string is a palindrome")
        print("Test Case:Pass")
    else:
        print("The given string is not a palindrome")
        print("Test Case:Pass") 
```
## OUTPUT

Alphanumeric values:

![Screenshot 2025-03-27 104904](https://github.com/user-attachments/assets/d834feef-578f-4be2-9905-c59a88025030)

Numeric values:

![Screenshot 2025-03-27 104933](https://github.com/user-attachments/assets/73468d2a-8b39-46b0-a0d5-431209ae173c)

Alphabet values:

![Screenshot 2025-03-27 104954](https://github.com/user-attachments/assets/027e4bf0-7697-4cae-9f11-7d98192443f8)

Non-palindrome string:

![Screenshot 2025-03-27 105022](https://github.com/user-attachments/assets/b11b70ca-8240-4702-8452-023dd3d2acde)

Symbols:

![Screenshot 2025-03-27 105053](https://github.com/user-attachments/assets/885e5c23-70ee-46a3-bb4f-2c6cbedc1335)


## RESULT
Thus, a program to check palindrome has been written and test cases have been written and verified
successfully.
