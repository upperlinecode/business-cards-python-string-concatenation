# Digital Business Cards

## The Goal

Let's create a program that prints out a beautiful command-line business card like this one:

![Example of User Input Cards](Concatenate.gif)

## Skills you may need

The following three major skills are really useful, but you may be able to at least _start_ without them. If you want to jump right into the lab, code your business card maker in the file called cards.py, and run it using the command `python cards.py`.

### User Input

In the example above, you can see that the user is entering three pieces of information about him/herself into the console.

Here's one example

```python
job = input("What is your position?") # the left side means we will store the user's position in a variable called job.
```

`input()` means, in plain English,  "whatever the user types in." So that line will store whatever the user enters as a string in a variable called job.

### Escape Sequences

You may want to store a string with some formatting in a variable. For example, consider these two ways of describing a dog:

###### Without escape sequences:
```python
# assign the variables:
description_line_1 = "Name: Maxine"
description_line_2 = "Breed: Puggle"
description_line_3 = "Color: Brown"
description_line_4 = "Weight: 12 lbs"

# print out the varibles:
print(description_line_1)
print(description_line_2)
print(description_line_3)
print(description_line_4)
```

###### With escape sequences:
```python
# assign all four lines to one variable:
full_description = "Name: Maxine \nBreed: Puggle \nColor: Brown \nWeight: 12 lbs"

# print out that variable:
print(full_description)
```

Believe it or not, those two blocks of code do the exact same thing. The "\n" sequence is the way to say "new line" while inside of a string literal. It lets you insert a line break without actually pressing the return button.

You may want to use "\n" and "\t" in your code to insert new lines and to tab information in from the side; these escape sequences can help you format your business cards.

### Concatenation and String Formatting.

One last skill you may need is concatenation. You can tell from the example that we won't know the user's job until they type it in, but the program has to be finished before you can run it and get the user to type it in.

The way we delay this information is with a "fill in the blank" style of writing code. If you want to print out the sentence "Hello! My name is ______. Welcome!", but with the blank filled in with the contents of a variable called name, that code can be done either of two ways.

###### With concatenation:

```python
"Hello! my name is " + name + ". Welcome!"
```

###### With string formatting:

```python
"Hello! my name is %s. Welcome!" % name
```

While either of these two strategies can work really well, concatenation often leads to a more readable line of code, and makes it easier to catch formatting errors. String formatting, on the other hand, has a lot of utility that will become more apparent the further we get into this course. Feel free to use whichever makes more sense to you.
