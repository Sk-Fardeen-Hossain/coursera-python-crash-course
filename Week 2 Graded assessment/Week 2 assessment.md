**1.**

Question 1

Complete the code to output the statement, “192.168.1.10 is the IP address of Printer Server 1”. Remember that precise syntax must be used to receive credit.

IP\_address = "192.168.1.10"

host\_name = "Printer Server 1"

print(IP\_address + " is the IP address of " + host\_name)

# Should print "192.168.1.10 is the IP address of Printer Server 1"

**Correct**

Correct.

**2.**

Question 2

What's the value of this Python expression: **"big" > "small"**?

**0 / 1 point**

True

False

big

small

**Incorrect**

Please review the “[Comparison Operators with Strings](https://www.coursera.org/learn/python-crash-course/supplement/Ut1Pe/comparison-operators-with-strings "Link to the Comparison Operators with Strings reading")” reading.

**3.**

Question 3

What directly follows the elif keyword in an elif statement?

**1 / 1 point**

A comparison

A colon

A logical operator

A function definition

**Correct**

**4.**

Question 4

Consider the following scenario about using if-elif-else statements:

Police patrol a specific stretch of dangerous highway and are very particular about speed limits. The speed limit is 65 miles per hour. Cars going 80 miles per hour or more are given a “Reckless Driving” ticket. Cars going more than 65 miles per hour are given a “Speeding” ticket. Any cars going less than that are labeled “Safe” in the system. 

Fill in the blanks in this function so it returns the proper ticket type or label.

def speeding\_ticket(speed):

`    `if speed>=80:

`        `ticket = "Reckless Driving"

`    `elif speed>65:

`        `ticket = "Speeding"

`    `else:

`        `ticket = "Safe"

`    `return ticket

print(speeding\_ticket(87)) # Should print Reckless Driving

print(speeding\_ticket(66)) # Should print Speeding

print(speeding\_ticket(65)) # Should print Safe

print(speeding\_ticket(85)) # Should print Reckless Driving

print(speeding\_ticket(35)) # Should print Safe

print(speeding\_ticket(77)) # Should print Speeding

**Correct**

Correct.

**5.**

Question 5

In the following code, what would be the output?

test\_num = 12

if test\_num > 15:

`    `print(test\_num / 4)

else:

`    `print(test\_num + 3)




15

3

12

4

**Correct**

**6.**

Question 6

Fill in the blanks to complete the function. The character translator function receives a single lowercase letter, then prints the numeric location of the letter in the English alphabet. For example, “a” would return 1 and “b” would return 2. Currently, this function only supports the letters “a”, “b”, “c”, and “d” It returns "unknown" for all other letters or if the letter is uppercase.

def letter\_translator(letter):

`    `if letter == "a":

`        `letter\_position = 1

`    `elif letter == "b":

`        `letter\_position = 2

`    `elif letter == "c":

`        `letter\_position = 3

`    `elif letter == "d":

`        `letter\_position = 4

`    `else:

`        `letter\_position = "unknown"

`    `return letter\_position

print(letter\_translator("a")) # Should print 1

print(letter\_translator("b")) # Should print 2

print(letter\_translator("c")) # Should print 3

print(letter\_translator("d")) # Should print 4

print(letter\_translator("e")) # Should print unknown

print(letter\_translator("A")) # Should print unknown

print(letter\_translator("")) # Should print unknown

**Correct**

Correct

**7.**

Question 7

Can you calculate the output of this code?

def difference(x, y):

`    `z = x - y

`    `return z

print(difference(5, 3))


2

**Correct**

**8.**

Question 8

What's the value of this Python expression?

**((24 == 5\*2) and (24 > 3\*5) and (2\*6 == 12))**

**1 / 1 point**

True

False

15

10

**Correct**

**9.**

Question 9

Fill in the blanks to complete the function. The “make\_positive” function takes in a number and converts that number to its positive equivalent.  Complete the function to accomplish the following tasks:

- use an if statement to test if the number is negative;
- use a calculation inside the if statement to change the negative number to be positive;
- use a calculation in the else statement to return any positive “number” unchanged.
- def make\_positive(number):
- `    `if number <0:
- `        `result = number \* -1 
- `    `else:
- `        `result = number
- `    `return result

- print(make\_positive(-4))   # Should print 4
- print(make\_positive(0))    # Should print 0
- print(make\_positive(-.25)) # Should print 0.25
- print(make\_positive(5))    # Should print 5
- **Correct**
- Correct.
- **10.**
- Question 10
- What are some of the benefits of good code style? Select all that apply.
- **0.75 / 1 point**

- Easier to maintain
- **Correct**

- Makes the intent of the code obvious

- Allows it to never have to be touched again

- Makes sure the author will refactor it later
- You didn’t select all the correct answers

