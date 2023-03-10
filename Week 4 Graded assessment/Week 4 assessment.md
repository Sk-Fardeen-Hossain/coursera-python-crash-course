**1.**

Question 1

The format of the input variable “address\_string” is: numeric house number, followed by the street name which may contain numbers and could be several words long (e.g., "123 Main Street", "1001 1st Ave", or "55 North Center Drive"). 

Complete the string methods needed in this function so that input like "123 Main Street" will produce the output "House number 123 on a street named Main Street". This function should:

1. accept a string through the parameters of the function;
1. separate the address string into new strings: house\_number and street\_name; 
1. return the variables in the string format: "House number X on a street named Y". 
1. def format\_address(address\_string):
1. `    `house\_number = ""
1. `    `street\_name = ""

1. `    `# Separate the house number from the street name.
1. `    `address\_parts = address\_string.split()

1. `    `for address\_part in address\_parts:
1. `        `# Complete the if-statement with a string method.
1. `        `if address\_part.isnumeric():
1. `            `house\_number = address\_part
1. `        `else:
1. `            `street\_name += " " + address\_part
1. `    `# Remove the extra space at the end of the last "street\_name".
1. `    `street\_name = street\_name.strip()

1. `    `# Use a string method to return the required formatted string.
1. `    `return "House number {} on a street named {}".format(house\_number, street\_name)

1. print(format\_address("123 Main Street"))
1. # Should print: "House number 123 on a street named Main Street"

1. print(format\_address("1001 1st Ave"))
1. # Should print: "House number 1001 on a street named 1st Ave"

1. print(format\_address("55 North Center Drive"))
1. # Should print "House number 55 on a street named North Center Drive"
1. **Correct**
1. Correct
1. **2.**
1. Question 2
1. Fill in the blank to complete the “string\_words” function. This function should split up the words in the given “string” and return the number of words in the “string”. Complete the string operation and method needed in this function so that a function call like "string\_words("Hello, World")" will return the output "2".
1. def string\_words(string):
1. `    `# Complete the return statement using both a string operation and 
1. `    `# a string method in a single line.
1. `    `return len(string.split())

1. print(string\_words("Hello, World")) # Should print 2
1. print(string\_words("Python is awesome")) # Should print 3
1. print(string\_words("Keep going")) # Should print 2
1. print(string\_words("Have a nice day")) # Should print 4

**Correct**

Correct

**3.**

Question 3

Consider the following scenario about using Python lists: 

Employees at a company shared  the distance they drive to work (in miles) through an online survey. These distances were automatically added by Python to a list called “distances” in the order that each employee submitted their distance. Management wants the list to be sorted in the order of the longest distance to the shortest distance. 

Complete the function to sort the “distances” list. This function should:

1. sort the given “distances” list, passed through the function’s parameters; ; 
1. reverse the sort order so that it goes from the longest to the shortest distance;
1. return the modified “distances” list.
1. def sort\_distance(distances):
1. `    `distances.sort()# Sort the list
1. `    `distances.reverse() # Reverse the order of the list
1. `    `return distances

1. print(sort\_distance([2,4,0,15,8,9]))
1. # Should print [15, 9, 8, 4, 2, 0]
1. **Correct**
1. Correct
1. **4.**
1. Question 4
1. Fill in the blank to complete the “increments” function. This function should use a list comprehension to create a list of numbers incremented by 2 (n+2). The function receives two variables and should return a list of incremented consecutive numbers between “start” and “end”* **inclusively** *(meaning the range should include both the “start” and “end” values).* Complete the list comprehension in this function so that input like “squares(2, 3)” will produce the output “[4, 5]”.
1. def increments(start, end):
1. `    `return [x for x in range(start+2,end+3)] # Create the required list comprehension.

1. print(increments(2, 3)) # Should print [4, 5]
1. print(increments(1, 5)) # Should print [3, 4, 5, 6, 7]
1. print(increments(0, 10)) # Should print [2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
1. **Correct**
1. Correct
1. **5.**
1. Question 5
1. Fill in the blanks to complete the “car\_listing” function. This function accepts a “car\_prices” dictionary. It should iterate through the keys (car models) and values (car prices) in that dictionary. For each item pair, the function should format a string so that a dictionary entry like ““Kia Soul“:19000” will print "A Kia Soul costs 19000 dollars". Each new string should appear on its own line.
1. def car\_listing(car\_prices):
1. `  `result = ""
1. `  `# Complete the for loop to iterate through the key and value items 
1. `  `# in the dictionary.
1. `  `for models,price in car\_prices.items():
1. `    `result += "A {} costs {} dollars ".format(models,price)+"\n"# Use a string method to format the required string. 
1. `  `return result

1. print(car\_listing({"Kia Soul":19000, "Lamborghini Diablo":55000, "Ford Fiesta":13000, "Toyota Prius":24000}))

1. # Should print:
1. # A Kia Soul costs 19000 dollars
1. # A Lamborghini Diablo costs 55000 dollars
1. # A Ford Fiesta costs 13000 dollars
1. # A Toyota Prius costs 24000 dollars

**6.**

Question 6

Consider the following scenario about using Python dictionaries: 

Tessa and Rick are hosting a party. Together, they sent out invitations, and collected the responses in a dictionary, with names of their friends and the number of guests each friend will be bringing. 

Complete the function so that the “check\_guests” function retrieves the number of guests (value)  the specified friend “guest” (key) is bringing. This function should:

1. accept a dictionary “guest\_list” and a key “guest” variable passed through the function parameters;
1. print the values associated with the key variable.
1. def check\_guests(guest\_list, guest):
1. `  `return guest\_list[guest] # Return the value for the given key

1. guest\_list = { "Adam":3, "Camila":3, "David":5, "Jamal":3, "Charley":2, "Titus":1, "Raj":6, "Noemi":1, "Sakira":3, "Chidi":5}

1. print(check\_guests(guest\_list, "Adam")) # Should print 3
1. print(check\_guests(guest\_list, "Sakira")) # Should print 3
1. print(check\_guests(guest\_list, "Charley")) # Should print 2

**Correct**

Correct

**7.**

Question 7

Complete the function so that input like "This is a sentence." will return a dictionary that holds the count of each letter that occurs in the string: {'t': 2, 'h': 1, 'i': 2, 's': 3, 'a': 1, 'e': 3, 'n': 2, 'c': 1}. This function should:

1. accept a string “text” variable through the function’s parameters;
1. iterate over each character the input string to count the frequency of each letter found, (only letters should be counted, do not count blank spaces, numbers, or punctuation; keep in mind that Python is case sensitive);
1. populate the new dictionary with the letters as keys, ensuring each key is unique, and assign the value for each key with the count of that letter;
1. return the new dictionary.
1. def count\_letters(text):
1. `  `# Initialize a new dictionary.
1. `  `dictionary = {}
1. `  `text=text.lower()
1. `  `# Complete the for loop to iterate through each "text" character and
1. `  `# use a string method to ensure all letters are lowercase.
1. `  `for letter  in text:
1. `    `# Complete the if-statement using a string method to check if the
1. `    `# character is a letter.
1. `    `if letter.isalpha() and letter not in dictionary:
1. `      `# Complete the if-statement using a logical operator to check if
1. `      `# the letter is not already in the dictionary.
1. `           `# Use a dictionary operation to add the letter as a key
1. `           `# and set the initial count value to zero.
1. `           `dictionary[letter] = text.lower().count(letter)
1. `      `# Use a dictionary operation to increment the letter count value
1. `      `# for the existing key.
1. `      `# Increment the letter counter.
1. `  `return dictionary

1. print(count\_letters("AaBbCc"))
1. # Should be {'a': 2, 'b': 2, 'c': 2}

1. print(count\_letters("Math is fun! 2+2=4"))
1. # Should be {'m': 1, 'a': 1, 't': 1, 'h': 1, 'i': 1, 's': 1, 'f': 1, 'u': 1, 'n': 1}

1. print(count\_letters("This is a sentence."))
1. # Should be {'t': 2, 'h': 1, 'i': 2, 's': 3, 'a': 1, 'e': 3, 'n': 2, 'c': 1}
1. **Correct**
1. Correct
1. **8.**
1. Question 8
1. What do the following commands return when genre = "transcendental"?
1. print(genre[:-8])
1. print(genre[-7:9])


1. endental, tr

1. transc, nd

1. ran, ental

1. dental, trans
1. **Correct**
1. **9.**
1. Question 9
1. What does the list "music\_genres" contain after these commands are executed?
1. music\_genres = ["rock", "pop", "country"]
1. music\_genres.append("blues")


1. ['rock', 'pop', 'blues']

1. ['rock', 'pop', 'country', 'blues']

1. ['rock', 'blues', 'pop', 'country']

1. ['rock', 'blues', 'country']
1. **Correct**
1. **10.**
1. Question 10
1. What do the following commands return?
1. speed\_limits = {"street": 35, "highway": 65, "school": 15}
1. speed\_limits["highway"]


1. 65

1. {"highway": 65}

1. [65]

1. ["highway", 65]
1. **Correct**

