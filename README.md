# Learning to Program by Using Swift

<br>
## Foreword

Most code blocks are elaborated upon in the first paragraph after the block, so read at least the trailing paragraph if the code block is confusing.

Each code block is independent of blocks before or after it.

Single quotes are used within paragraphs to talk about words and operators from code blocks.

<br>
## Hello, World

In order to get acquainted with Swift, the very first thing you will learn to do is make your program say hello to you. So open up Xcode, create a new playground, and type the following:

```
print("Hello, World!")
```

At the very bottom of your playground, is a large, empty rectangle known as the console. The console is how your program will talk to you. When you put the above line of code in your playground, the console will output:

```
Hello, World!
```

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

You may have noticed the first line puts quotation marks around what it wants to print, while the second line does not. This is because the first line is printing a String--which is a series of letters, numbers or most any character you can think of. Meanwhile the second line is printing an Int(eger). Ints are a type of number and they are written without quotes. Here are some more examples:

```
// This is a comment. Anything you write after two slashes does not have to be code and will not cause errors

// The following are Strings
"Mason loves dogs."
"Mason also loves cats!"
"500" // It does not matter that a number is between the quotation marks. As long as there are quotes, it's a string.

// The following are Ints
256
720
0
```
Whether something is a String or an Int is known as its type. When we refer to something's type, we capitalize the type. Strings and Ints are two of the most fundamental types in Swift, and you'll come to learn about many more.

<br>
## Variables

We use variables so that our programs will work for multiple values and not only the ones we enter manually ourselves. You'll learn more about that in furture lessons. For now, though, let's learn how we make and use these variables.

A variable is like a box. Boxes generally hold things, and when you have many boxes, you want to give them labels so that you can tell which box is which. In Swift, you can label a box using the keyword 'var,' and you can put something inside of a box using the '=' sign. For now, anytime we label a box, we will also put something inside of it. Here is how:

```
var myBox = 5
```

Now let's break that down. The word 'var' is how you let the program know that you want to get a new box down from the shelf.  Whatever you put between 'var' and the '=' is your new box's label; in the above example, 'myBox' is the label. You can label the box almost anything you want (but, for example, you cannot label it 'var'). Finally, whatever you put after the '=' is what your new box will hold. This box holds the Int 5.

What can you do once you have this variable? Well one thing you can do is print it, the same way we made our program say hello to us. Let's see that:

```
var myBox = 5
print(myBox)
```

The resulting console output will be:

```
5
```

This example shows that when the program tries to print the output to the console, it translates any variables to their actual values. Keep in mind that if you were to put quotes around the variable name, the program would see it as simply a String and printing it would treat it as such. Here's an example:

```
var myBox = 10
print(myBox)
print("myBox")
print(myBox)
```

The console output would be:

```
10
myBox
10
```

One important thing to remember is that once you label a box with a certain name, you cannot label another box with the same name. If you did that and then I asked you to grab me the box labled 'blue,' you wouldn't know which one I mean. Consequently, the following program is illegal:

```
var myBox = 10
var myBox = 20 // the Playground will put a red circle here and tell you that myBox has been redeclared
```

What you can do with a standard box once it's labeled is replace what's inside it. You replace what's inside it using the '=' operator, just as you did to give it its initial contents. See the following:

```
var myBox = 10
myBox = 20 // the Playground allows this, because you're only altering the contents of the existing box, not grabbing a new one
```

To elaborate on how this program will be run, let's add some print statements as in the following:

```
var myBox = 10
print(myBox)
myBox = 20
print(myBox)
```

The console output will be:

```
10
20
```

To explain, at the first print, the box labeled 'myBox' contains the 10 initially put into it so '10' is printed. After that first print statement, the 10 is taken out of the box and 20 replaces it. Thus when print is called with 'myBox' the second time, it contains 20 at that point.

Now you may want to try changing the variable as in the following example:

```
var myBox = 20
myBox = "I need new headphones" // the Playground will give you an error for this.
```

Unforunately, this won't work
