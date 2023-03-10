**1.**

Question 1

Fill in the blanks to print the numbers from 15 to 5, counting down by fives.

number = 15 # Initialize the variable

while (number>=5): # Complete the while loop condition

`    `print(number, end=" ")

`    `number -=5# Increment the variable

# Should print 15 10 5 

**Correct**

Correct

**2.**

Question 2

Find and correct the error in the **for** loop below.  The loop should check each number from 1 to 5 and identify if the number is odd or even. 

for number in range(5):

`    `if number % 2 == 0:

`        `print("odd")

`    `else:

`        `print("even")

# Should print:

# odd

# even

# odd

# even

# odd

**Correct**

Correct

**3.**

Question 3

Fill in the blanks to complete the function “even\_numbers(n)”. This function should count how many even numbers exist in a sequence from 0 to the given “n”number, where 0 counts as an even number. For example, even\_numbers(25) should return 13, and even\_numbers(6) should return 4.

def even\_numbers(n):

`    `count = 0

`    `current\_number = 0

`    `while current\_number<=n: # Complete the while loop condition

`        `if current\_number % 2 == 0:

`            `count+=1 # Increment the appropriate variable

`        `current\_number+=1 # Increment the appropriate variable

`    `return count



print(even\_numbers(25))   # Should print 13

print(even\_numbers(144))  # Should print 73

print(even\_numbers(1000)) # Should print 501

print(even\_numbers(0))    # Should print 1

**Correct**

Correct

**4.**

Question 4

Fill in the blanks to complete the “sequence” function. This function should print a sequence of numbers in descending order, from the given "high" variable to the given "low" variable.  The range should make the loop run two times. Complete the range sequences in the nested loops so that the “sequence(1, 3)” function call prints the following:

3, 2, 1

3, 2, 1

def sequence(low, high):

`    `# Complete the outer loop range to make the loop run twice

`    `# to create two rows

`    `for x in range(0,3): 

`        `# Complete the inner loop range to print the given variable

`        `# numbers starting from "high" to "low" 

`        `# Hint: To decrement a range parameter, use negative numbers

`        `for y in range(high,-low): 

`            `if y ==high:

`                `# Don’t print a comma after the last item

`                `print(str(y)) 

`            `else:

`                `# Print a comma and a space between numbers

`                `print(str(y), end=", ") 

sequence(1, 3)

# Should print the sequence 3, 2, 1 two times, as shown above.

**Incorrect**

Please review the "More for Loop Examples" and the "Nested

for Loops" videos.

**5.**

Question 5

Fill in the blanks to complete the “counter” function. This function should count down from the “start” to “stop” variables when “start” is bigger than “stop”. Otherwise, it should count up from “start” to “stop”. Complete the code so that a function call like “counter(3, 1)” will return “Counting down: 3, 2, 1” and “counter(2, 5)” will return “Counting up: 2, 3, 4, 5”.

def counter(start, stop):

`    `x = start

`    `if x>stop:

`        `return\_string = "Counting down: "

`        `while x >= stop:

`            `return\_string += str(x)

`            `if x>stop:

`                `return\_string += ","

`            `x = x-1

`    `else:

`        `return\_string = "Counting up: "

`        `while x <= stop:

`            `return\_string += str(x)

`            `if x<stop:

`                `return\_string += ","

`            `x = x+1

`    `return return\_string

print(counter(1, 10)) # Should be "Counting up: 1,2,3,4,5,6,7,8,9,10"

print(counter(2, 1)) # Should be "Counting down: 2,1"

print(counter(5, 5)) # Should be "Counting up: 5"

**Correct**

Correct

**6.**

Question 6

Fill in the blanks to complete the “odd\_numbers” function. This function should return a space-separated string of all odd positive numbers, up to and including the “maximum” variable that's passed into the function. Complete the for loop so that a function call like “odd\_numbers(6)” will return the numbers “1 3 5”.

def odd\_numbers(maximum):



`    `return\_string = "" # Initializes variable as a string

`    `# Complete the for loop with a range that includes all 

`    `# odd numbers up to and including the "maximum" value.

`    `for x in range(1,maximum+1):

`        `if x%2==1:

`            `return\_string += str(x) + " "  

`    `# This .strip command will remove the final " " space 

`    `# at the end of the "return\_string".

`    `return return\_string.strip()

print(odd\_numbers(6))  # Should be 1 3 5

print(odd\_numbers(10)) # Should be 1 3 5 7 9

print(odd\_numbers(1))  # Should be 1

print(odd\_numbers(3))  # Should be 1 3

print(odd\_numbers(0))  # No numbers displayed

**Correct**

Correct

**7.**

Question 7

The following code is supposed to add together all numbers from x to 10. The code is returning an incorrect answer, what is the reason for this?

x = 1

sum = 5

while x <= 10:

`    `sum += x

`    `x += 1

print(sum)

# Should print 55




Should use a for loop instead of a while loop 

Not incrementing the iterator (x)

The code is not inside of a function

The "sum" variable is initialized with the wrong value

**Correct**

**8.**

Question 8

How many numbers will this loop print? Your answer should be only one number.

for sum in range(5):

`    `sum += sum

`    `print(sum)

**Incorrect**

Please review the “[More for Loop Examples](https://www.coursera.org/learn/python-crash-course/lecture/00vRH/more-for-loop-examples)” video and the “[A Closer Look at the Range() Function](https://www.coursera.org/learn/python-crash-course/supplement/8yePF/a-closer-look-at-the-range-function)” reading.

**9.**

Question 9

What is the initial value of the “outer\_loop” variable on the first iteration of the nested "inner\_loop"? Your answer should be only one number. 

for outer\_loop in range(2, 6+1):

`    `for inner\_loop in range(outer\_loop):

`        `if inner\_loop % 2 == 0:

`            `print(inner\_loop)

**Correct**

**10.**

Question 10

The following code causes an infinite loop. Can you figure out what’s missing and how to fix it?

def count\_numbers(first, last):

`  `# Loop through the numbers from first to last 

`  `x = first

`  `while x <= last:

`    `print(x)

count\_numbers(2, 6) 

# Should print:

# 2

# 3

# 4 

# 5

# 6




Missing the break keyword

Variable x is not incremented

Wrong comparison operator is used

Missing an **if-else** block

**Correct**


