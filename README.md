# Learn to Code: Introduction to Python

Brought to you by Galvanize. Learn more about the way we teach at [galvanize.com](http://galvanize.com).

Get to this repo by typing in URL: **https://github.com/nkrao220/intro-to-python**

### FAQ: 

- WIFI: 'GEvents` | Password: GEvents1644
- Restrooms: Behind you down the hall to the right
- Kitchen outside with Coffee,Tea, and Pizza!

## Overview
The goal of this brief course is to provide you with a fun introduction to the world of development with Python.

#### Here's what we'll be doing:
* Overview of basic Python and programming concepts
* Building a simple application using Python
* Playing around and break things


#### What is programming?
Programming is giving your computer a set of instructions to perform a task. 

This sounds simple but it can get complicated! 


## Setting up your computer


#### Please set up the following:

* A web browser to see what we're working on as others see it (Recommend Google Chrome: [chrome.google.com] (http://chrome.google.com))
* We will be using an online text editor for this workshop. You can sign up here: [https://repl.it/](https://repl.it/)


Well... that was easy! 


## What this workshop is

A super friendly introduction to Python No previous experience expected! 

You can't learn EVERYTHING in ~2 hours. But you can learn enough to get excited and comfortable to keep working and learning on your own! 

- This course is for absolute beginners
- Ask Questions!
- Answer Questions!
- Help others when you can
- Its ok to get stuck, just ask for help!
- Feel free to move ahead
- Be patient and nice

### Challenges:
Get the most out of this workshop! We'll occasionally do a "CHALLENGE" where I give you an exercise to do in several minutes. It can be even more effective to partner up with someone next to you, but you can work on your own if you want. No pressure to solve the challenge. I'll share how I would solve it after the time is up.


## About me:

Neha Rao - associate data science instructor - data scientist 
https://www.linkedin.com/in/neha-k-rao/



## About you!

Give a quick Intro!

- Whats your name?
- Whats your background?
- Why are you interested in Python?

## What is Python?

### A VERY brief history

Created by Guido van Rossum and released in 1991.

Python is Known ease of learning, code readability (must use code indents), and a massive ecosystem of libraries that easily expand its usefulness is many fields.

Read more about the history of Python [here](https://en.wikipedia.org/wiki/Python_(programming_language)).


### Who uses Python?

A lot of places do!

- Large Companies (Google, Facebook)
- Startups
- Agencies
- Majority of companies doing data science 

### What can you do with Python

- Web Development
	- Back-End (frameworks: Django, Flask, more)
- Data Science and AI
	- Data Analysis
	- Machine Learning
	- Deep Learning
	- Computer Vision
	- Natural Language Processing
- [Embedded(Hardware)](https://micropython.org/)
- Devops

#### Popular Frameworks and libraries to keep in mind

When learning more about Python you'll probably see some of these pop up as you continue to study

- Web
	- Django
	- Flask
	- pyramid

- Data Science
	- Tensorflow
	- Keras
	- Numpy
	- Pandas
	- Scikit Learn
	- OpenCV

*Note*: if you're thinking of exploring data science with python look into using [Anaconda](https://www.anaconda.com/) to manage your python and data libraries

Also [Google Colab](https://colab.research.google.com/notebooks/welcome.ipynb#recent=true) is a awesome place to start as well without having to install anything!


## Python Basics:

### Printing
`print("Hello, Galvanize")`

### Variables:
Variable are a way to store information.
This is super useful! You can then receive or update the variable in your program. You'll see this later!

Think of it as naming a piece of data.

its common in programming languages to have a keyword before the variable such as `var` or `int`, but python does not need this. 

- `twitter = "@sagecodes";`
- `score = 0;`

--------

### Challenge:

Create a variable called `name` and assign it your name.
Use the `print()` function to print out the variable value.

-------

### Data Types:
We're going to stick with the basics, so We wont be going over EVERY data type in Python, but you you can read a more comprehensive list [here](https://docs.python.org/3/library/stdtypes.html#dict).  

Feel free to try these different data types out in your code!

#### Numbers:

Numbers are written just like you would think. Just the number! No quotes or symbols to worry about. If you do put quotes around a number it will become a string (see next)

`25` `100`

Multiply, Add, Divide, Compare, remainder

- `5 * 5` | output: 25
- `5 + 5` | output: 10
- `8 / 2` | output: 4
- `8 > 2` | output: true
- `8 % 8` | output: 0 

#### Strings:
Strings can be a collection of letters, symbols and/or numbers. They are made by surrounding the content with quotation marks.

`"Hello, World."`
`"CrAzy Random String 987879896jvdjvda &&(&(@*(*"`

can use double: ", Single ' or triple(3 singles) ''' quotes for strings.

Can we add strings together? Try it out!

##### Variables in strings

How can we add variables into our strings

```
varOne = "VAR1"
varTwo = "VAR2"
varThree = "VAR3"

# concatenation 
string1 =  "this is a string" + varOne + "More string"

# More common way
string2 =  "this is a string {} More {} string".format(varOne, varTwo)

# you can specify which variable is used where
string3 =  "varTwo is: {1} varOne is: {0}".format(varOne, varTwo)

print(string3)

```

```
intOne = 5
floatOne = 6.6222
boolOne = True


# This format is helpful because it knows you want a string value for other types of data. 
string2 =  "These all get converted when using this format {} {} {}".format(intOne, floatOne, boolOne)

print(string2)
```

##### slicing

word[start:end] # items start through end-1
word[start:]    # items start through the rest of the string
word[:end]      # items from the beginning through end-1

```
word = "batman"

print(word[1:3])
print(word[3:])
print(word[:3])

```

Fun thing with [extended slicing](https://docs.python.org/2/whatsnew/2.3.html)

an easy way to reverse a string by adding a step!

```
word = "batman"
print(word[::-1])

```



---
### Challenge:

- create a variable with the string "superman"
- use slicing to only print out "super"
- can you reverse it?

---



#### Booleans:
You can think of Booleans as yes(true) and no(false)

`True` `False`

We'll go into how to use these in a little bit. For now just remember they exist!


#### Lists (Arrays)

Often used to store a list of values.

```
tvshows = ['West World','Mr. Robot', 'Game of Thrones']
print(tvshows)
```

print single item. Index starts at zero

```
print(tvshows[0])
```

##### Update an item in an array
```
tvshows[0] = "killer robots"
```
##### Add to an array

```
tvshows.append("FireFly")
print(tvshows)
```

##### Remove from an array

```
tvshows.remove("Game of Thrones")
print(tvshows)
```

Or if you want to get rid of a certain part of the list

```
tvshows.remove(tvshows[0])
print(tvshows)
```

read more about python lists[here](https://www.w3schools.com/python/python_lists.asp).

#### Tuples

Tuples behave a lot like lists, except you can't change the values


```
tvshows = ('West World','Mr. Robot', 'Game of Thrones')
print(tvshows)
```
you cannot update tuples in your code. They will throw an error.


#### Dictionary (Dict)

Dictionaries can also be used to store values, but they are indexed. 


```
person =	{
  "name": "Bob",
  "age": 50,
  "occupation": 'programmer'
}
print(person)
print(person['name'])

```


##### update

```
person['name'] = "Ted"
print(person['name'])
```

##### add
```
person['city'] = 'Seattle'  
print(person)
```

##### remove

```
del person['age']
print(person)
```

read more about python dictionaries[here](https://www.w3schools.com/python/python_dictionaries.asp).

-------
### Challenge:
- make a list `[]` containing your favorite foods.
- update the list adding more item
- remove the first item from the list

- Make dictionary with values about your self.
- update one of the values
- add a new value
- remove one of the values

-------



## Comparison Operators:
Comparison Operators are used quite frequently in programming. Its a great way to compare and use data.

Again we won't cover ALL of the comparison operators in this workshop, but you can see a full list of them [here](https://docs.python.org/3/library/stdtypes.html#comparisons)

- `==` Equal
- `!=` Not Equal
- `>` Greater Than
- `>=` Greater Than or Equal
- `<` Less Than
- `<=` Less Than or Equal

Example:

`current_score >= highest_score`
This would return a boolean value. Depending on the values of these variables this would return either `True` or `False`. Try it in your console using numbers instead of variables!


## Spacing
most of the upcoming examples you'll see parts of the code indented.
This lets python know when blocks of code begin & end. I'll explain as we go through examples. Just remember that spacing is important and it can cause issues with your code working.


## Conditionals

When writing a program you'll often want to check if data meets a certain condition or not. We can use conditionals to make decision about our data and create different outcomes

 In javascript you'll often use the `if` statement. This may be followed by `else if` or `else` depending on how many conditions need to be checked.

Example:

```
 if guess == answer:
      message = "You Win!"
  elif guess < answer:
      message = "Your guess is too low!"
  elif guess > answer:
      message = "your guess is too high!";
  else:
    message = "I think you entered something wrong..."

```

---
### challenge

- make a variable with with a numerical value. 
- using the `if`, `elif`, and `else` make your program print something different depending on the value in your variable.

---

## Loops
We're going to go over some of the basic loops in python, but yet again we're not going to cover everything, so you may want to read more about loops [here](https://www.learnpython.org/en/Loops).

Loops are used when you want to repeat something. You can repeat the exact same thing, or change some variable and repeat the action again.

the two common types of loops are `for` and `while`.
`for` loops are often used to run a loop a specified amount of time.

`while` loops are often used to run a loop indefinitely until certain criteria are met.

Example:

This `for` loop will run 5 times, and print out the value of `x` to the console. 

for loop:

```
for x in range(5):
    print(x)
```

For loops are often used to loop through variables containing lists and dicts to get the individual values stored in them. 

Try running these:
```
arr = [1,"hi",6,6]
for x in arr:
    print(x)
```    
```    
word = "Hello"
arr = [1,"hi",6,6]
for x in word:
    print(x)
```

```
info = {'name': 'sage', 
        'language':"python" }
for x in info:
    print(info[x])
```

read more on for loops [here](https://www.w3schools.com/python/python_for_loops.asp)

while loop:

```
count = 1
while count <= 5:
    print(count)
    count += 1  # This is the same as count = count + 1
```


read more on while loops [here](https://www.w3schools.com/python/python_while_loops.asp)

---
### challenge
[Fizzbuzz](https://en.wikipedia.org/wiki/Fizz_buzz) and variations of it is a popular interview question. 

"From 1 to 100.

For each multiple of 3, print "Fizz" instead of the number. 

For each multiple of 5, print "Buzz" instead of the number. 

For numbers which are multiples of both 3 and 5, print "FizzBuzz" instead of the number."

Lets break it down and solve it together!

---

## Iterating

Now that we know about loops lets talk a bit about iteration! 

Many objects may have data we want to iterate through to do something with it. Common iterables: Strings, Lists, Dicts, tuples.

String:

```
word = "hello"

for x in word:
	Print(x)
```

lists:

```
tvshows = ['West World','Mr. Robot', 'Game of Thrones']

for x in tvshows:
	print(x)
```

Dictionaries 

```
person =	{
  "name": "Bob",
  "age": 50,
  "occupation": 'programmer'
}

# get the values
for x in person:
	print(person[x])
	
# get the keys
for x in person:
	print(x)
	
```

## Functions
Reduce, Reuse, Recycle

Functions make it easy to reuse code. If you find yourself repeating code you may want to turn it into a function!

Example:
This function takes in two arguments(a, b) and returns the value of them added together. 

```
def add(a, b):
	print(a + b)
```
to use the function call it by writing its name and open/close parenthesis(). With arguments passed inside the parenthesis():

- `add(5,5)` | output: 10
- `add(2,5)` | output: 7

In this simple example you're not saving a ton of code, but imagine a function that uses many lines of code! 

Scope example?

---
### challenge

Create a function that multiplies 3 numbers together and prints out the values.

Make out fizzbuzz solution a function that takes an input for the range of fizzbuzz

---


## Interact with users

Getting input from the command line can be useful.

To do that we will use the `input` function. And we want to assign that input to a variable.

`guess = input("enter guess")`

Print will output text to the terminal

```
guess = input("enter guess: ")
print("Your guess was {}".format(guess))
```

---
### Challenge:

Using the `input()` function ask a user for there name. Then print out a sentence using the name. 

---

## Comments

use a hashtag for comments.

`# this is a comment`

---
### Challenge:

If you saved your code from other challenges go back and comment what the code is doing.

---


## Review:

<details>
  <summary>What is a Variable</summary>
  
  A variable is something you can store information into.
	
</details>

<details>
  <summary>What are the three common ways to declare a string</summary>
  
  'Single quotes'
  "Double quotes"
  '''Triple Single quotes'''
	
</details>

<details>
  <summary>What is a Boolean?</summary>
  
  A boolean can be set to True or False. Yes and No.
	
</details>

<details>
  <summary>What is a List in python?</summary>
  
  A list can store multiple values in order. 
  
  ls = ["apples","oranges","bannas"]
	
</details>

<details>
  <summary>How is a Dictionary (Dict) in python different than a list?</summary>
  
  Dictionary has a key value pair. You usually interact with it by calling a key. `person['age']`
	
</details>

<details>
  <summary>What the difference between a for loop and a while loop?</summary>
  
  for loops are usually used to loop a certain amount of times
  
  while loops will loop until a condition is met.
	
</details>

<details>
  <summary>What is a function in Python?</summary>
  
  A function is a chunk of code that you can reuse and pass data into
	
</details>

<details>
  <summary>How do you make a comment in Python?</summary>
  
 # use the # in front of it
	
</details>

<details>
  <summary>What is a conditional in Python?</summary>
  
 A way to check if data meets a certain condition or not. `if` `elif` `else`.
	
</details>

<details>
  <summary>What does the `%` Modulo do?</summary>
  
The modulo return the remainder 
	
</details>


## Lets do some code!
You just learned a lot! Lets put it together and build something!

Sign up if you haven't already and create a new project: https://repl.it/


We're going to build a number guessing game using:

- variables
- Comparison Operators
- Conditionals
- loops
- functions
- dialog boxes

If you get stuck or want to look ahead at the completed project you can view it [here](https://repl.it/@SageElliott/pythonGuessingGame).

What are some ideas for improvements? 

- Exit on command
- data validation
- input the number range from popup
- output grammar depending on number of tries



# YOU DID IT! YOU'RE NOW A PROGRAMMER!





### Welcome! :)

### Keep learning!


Learning resources:

- [Python Fundamentals: accelerated TUITION CREDIT AVAILABLE!!](https://www.eventbrite.com/e/python-fundamentals-accelerated-91619-10319-tickets-66397884861)

- [Intro to Data Science: Tuition Credit Available](https://www.eventbrite.com/e/intro-to-data-science-evening-intensive-tickets-65055755516)

- [Galvanize Data Science Prep Course](https://www.galvanize.com/data-science-prep) - FREE | study at your own pace

- [w3schools](https://www.w3schools.com/python/default.asp) | Free

- [Datacamp](https://www.datacamp.com/courses/intro-to-python-for-data-science) | Free

- [codecademy: learn-python](https://www.codecademy.com/learn/learn-python) | Free


## Upcoming Events!

We host so many events! check out our [calendar](https://www.galvanize.com/events)

Visit the [Learn to code Denver and Colorado Data Science](https://www.meetup.com/learn-to-code-colorado/) (https://www.meetup.com/Colorado-Data-Science/) meetup for all upcoming events.


[Web Scraping with Python](https://www.eventbrite.com/e/web-scraping-with-python-tickets-59851454311) 2hour workshop! 

## What is Galvanize?
###### We are a community!


#### Immersive Bootcamp

- [Data Science](https://www.galvanize.com/data-science)
- [Software Engineer](https://www.galvanize.com/web-development)

#### Part-Time Courses

- [Digital Marketing with Data](https://www.galvanize.com/part-time/digital-marketing)
- [Python Fundamentals](https://www.galvanize.com/part-time/data-science-fundamentals)
- [Introduction to Data Science] (https://www.galvanize.com/part-time/intro-to-data-science)


#### Co-working Space

[work in our building!](https://www.galvanize.com/entrepreneur)

#### We are a community

## Questions

Please feel free to reach out to me with any questions! Let me know what you're planning to do next and how I can help!


-LinkedIn 
-Email [neha.rao@galvanize.com]


Questions about education at Galvanize email [travis@galvanize.com](travis@galvanize.com)






