# Learning to Program by Using Swift

<br>
## Foreword

Each code block is independent of blocks before or after it.

Italics are used within paragraphs to talk about words and operators from code blocks.

<br>
## Hello, World!

In order to get acquainted with Swift, the very first thing you will learn to do is make your program say hello to you. So open up Xcode, create a new playground, and type the following:

```
print("Hello, World!")
```
At the very bottom of your playground, is a large empty empty rectangle known as the console. The console is how your program will talk to you. When you put the above line of code in your playground, the phrase _Hello, World!_ will appear in that console.

Whatever you put in between the parentheses is what your program will say to you. For example, this code:
```
print("I love learning!")
print(5)
```
will output the following to the console:
```
I love learning!
5
```
You may have noticed the first line puts quotation marks around what it wants to print, while the second line does not. This is because the first line is printing a String-which is a series of letters, numbers or most any character you can think of. Meanwhile the second line is printing an Integer. Integers don't need to be surrounded by quotes. Here are some more examples:
```
// This is a comment. Anything you write after two slashes does not have to be code and will not cause errors

// The following are Strings
"Mason loves dogs."
"Mason also loves cats!"
"500" // It does not matter that a number is between the quotation marks. As long as there are quotes, it's a string.

// The following are Integers
256
720
0
```
Whether something is a String or an Integer is known as its type. When we refer to something's type, we capitalize the type. Strings and Integers are two of the most fundamental types in Swift, and you'll come to learn about many more.

<br>
## Variables

A variable is a box that can hold something inside of it. When you have many boxes, you want to give them labels so that you can tell which box is which.

In Swift, you can put something inside of a labeled box using the _=_ sign. For now, whenever we label a box, we also want to put something inside of it. Here is how.

```
var myBox = 5
```
Now let's break that down. The word _var_ is how you let the program know that you want to get a new box down from the shelf.  Whatever you put between _var_ and the _=_ is your new box's label. In the above example, _myBox_ is the label. You can label the box almost anything you want (for example, you cannot label it _var_). Finally, whatever you put after the _=_ is what your new box will hold. This box holds the Integer 5.

What can you do once you have this variable? Well one thing you can do is _print_ it. Let's see how to do that:
```
var myBox = 5
print(myBox)
```
The resulting console output will be:
```
5
```
