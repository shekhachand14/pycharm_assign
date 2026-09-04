# pycharm_assign
# Write a program to reverse a string without using slicing.
Input = "python"
reverse = " "
for x in Input:
    reverse = x + reverse
print(reverse)

# Find the first non-repeating character in a string.
Input = "programming"
for x in Input:
     if  Input.count(x) == 1:
         print(x)

# Check if a string is a palindrome.
Input = "madam"
reverse = ""
for x in Input:
    reverse = x + reverse
if Input == reverse:
    print("True")
else:
    print("Not True")

# Q4 Count the frequency of each character in a string.
Input = "hello"
d ={}
for x in Input:
    if x in d:
        d[x] = d[x] + 1
    else:
        d[x] = 1
print(d)

# Q5 Remove duplicate characters from a string while preserving order.

Input = "programming"
d = {}
output = " "
for x in Input:
     if x not in d:
        d[x] = 1
        output = output + x
print(output)

# Q6 Remove duplicates from a list without using set().
Input = [1,2,2,3,4,4]
d = {}
output = [ ]
for x in Input:
    if x not in d:
        d[x] = 1
        output.append(x)
print(output)

# Find the second largest number in a list.
Input = [10,20,5,30,25]
Largest1 = Input[0]
Largest2 = Input[0]

for x in Input:
     if x > Largest1:
         Largest2 = Largest1
         Largest1 = x
     elif x > Largest2 and x != Largest1:
         Largest2 = x
print(Largest2)

# Q8 Find all duplicate elements in a list.
Input = [1,2,3,2,4,5,1]
d = {}
output = []
for x in Input:
   if x in d:
    if x not in output:
      output.append(x)
   else:
       d[x] = 1
print(output)

# Q9 Rotate a list by K positions.
Input = [1,2,3,4,5]
K = 2
output = []
for x in range(len(Input) - K, len(Input)):
    output.append(Input[x])

for x in range(0, len(Input) - K):
    output.append(Input[x])

print(output)

# Q10 Find the intersection of two lists.
Input1 = [1, 2, 3, 4]
Input2 = [3, 4, 5, 6]
Output = []
for x in Input1:
    if x in Input2:
        Output.append(x)
print(Output)

# Q11 Count frequency of elements in a list using a dictionary.
Input = [1,2,2,3,3,3]
d = {}
for x in Input:
    if x in d:
        d[x] = d[x] + 1
    else:
        d[x] = 1
print(d)

# Q12 Find the key having the maximum value.
Input = {"A":100,"B":500,"C":300}
max = 0
max_key = " "
for key in Input:
    value = Input[key]
    if value > max:
       max = value
       max_key = key
print(max_key)

# Q13 Reverse a dictionary.
Input = {"a":1,"b":2}
reverse = {}
for key in Input:
    reverse[Input[key]] = key
print(reverse)

# Q14 Merge two dictionaries.

d1 ={"a":1}
d2 ={"b":2}
output = {}
for key in d1:
    output[key] = d1[key]
for key in d2:
    output[key] = d2[key]
print(output)

#  Q15 Count word frequency in a sentence using dictionary.

Input = "python is good python is easy"
words = Input.split()
output ={}
for  x in words:
    if x in output:
        output[x] = output[x] + 1
    else:
        output[x] = 1
print(output)

# Print the following pattern:
for i in range(1,3):
      print("*" * i)

# Q17 Print multiplication table of a given number.
Input = 5
for i in range(1,11):
    print(Input, "x", i, "=", Input * i )

#  Q18 Find factorial using for loop.
Input = 5
factorial = 1
for i in range(1, Input + 1):
   factorial = factorial * i
print(factorial)

# Q19 Find all prime numbers between 1 and 100.
for pri_num in range(2,101):
     prime = True

     for i in range(2,pri_num):
         if pri_num % i == 0:
             prime = False

     if prime:
         print(pri_num)

#   Q20 Generate Fibonacci series up to N terms.
Input = 8
a = 0
b = 1
for i in range(Input):
     print(a, end=" ")
     c = a+b
     a = b
     b = c

# Q21 Find the first non-repeating number in a list.
Input = [1,2,3,4,5,1,2,3]
for x in Input:
     if Input.count(x) == 1:
        print(x)

# Q 22 Find the Nth non-repeating number in a list.
Input = [1, 2, 3, 4, 5, 1, 2, 3]
N = 2
count = 0
for x in Input:
    if Input.count(x) == 1:
        count = count + 1

        if count == N:
            print(x)

# Check whether two strings are anagrams.
#Input: “listen” “silent”
#Output: True
str1 = "listen"
str2 = "silent"
if sorted(str1) == sorted(str2):
       print(True)
else:
        print(False)

# Q24 Find missing number from array.
Input = [1, 2, 3, 5]
n = 5
total = 0
for x in Input:
    total = total + x
expected = 0
for i in range(1, n + 1):
    expected = expected + i
missing = expected - total
print(missing)

# 25 Find top occurring element in a list.
Input = [1, 2, 2, 3, 3, 3, 4]

max_count = 0
top_element = 0

for x in Input:
    count = Input.count(x)

    if count > max_count:
        max_count = count
        top_element = x

print(top_element)
