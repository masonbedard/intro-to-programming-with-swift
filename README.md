# Learning to Program by Using Swift

## Hello, World

Without wasting a moment, let's write our first Swift program. We'll begin by launching Xcode and choosing the option to create a new playground. You can give the playground any name you like, and you can decide on any save location (the default will work just fine). After hitting okay, you'll be met with a large, empty area where you're going to write your code.

To begin, delete everything in the playground except the line reading:
```
import UIKit
```
Now we can begin our program. Type the following on a new line:
```
100
```
Congratulations because you've just written code. It's true! The playground reads that '100' you just wrote, and it evaluates it. Evaluating a line means simplifying it as much as possible by performing any and all operations on that line. In this case, there are no operations to perform--there's only the number '100' that you wrote.

On the righthand side of the playground is a grey area that should at this point have '100' printed in it, lined up with the '100' you typed. This '100' that you didn't type is the result of the playground's evaluating that line. And as we mentioned, because there are no operations on this line, it simply evaluates to '100.' And it works the same for any number you care to try. Whether you type 13, 500 or 10000, you are writing code.

## Operations

Let's see how powerful this playground's evaluation can be. We'll start by trying some arithmetic. Type the following, one by one, into the playground:
```
90 + 90
4 * 8 - 10
120 / 4 + 6
```
After everything is entered, the first line should line up with a '180' in the grey panel on the right side of the playground. In Swift, '\*' means multiplication; therefore, the '4 * 8 - 10' should line up with a '22,' as standard order of operation rules apply. Finally '120 / 4 + 6' ought to line up with a '36.' Hopefully, you're starting to gain a better understanding of what evaluation means, and why these numbers and operators can be considered code.

## Variables

As you've seen, all the code you've written so far certainly gets evaluated. However, as of now the results of these evaluations are simply printed on the rightside of your playground, and then they disappear. Basically, by the time the next line is being evaluated, the previous line is history. So let's not forget our history (because otherwise, just as in the real world, we'd be doomed to repeat it). 

A way we can do that is by storing evaluation results in variables. A variable is like a container that you label so that you can always come back to it, identify it and use whatever it holds inside. Let's see how you do this in code:
```
let container = 90 + 90
```
The '90 + 90,' part should look familiar to you as it's one of the first lines of code we wrote together. As you may remember, when '90 + 90' is the only text on the line, the program evaluates it to be 180. In an identical fashion, the first thing the program does when it reads this line is to evaluate that '90 + 90' as 180 again. What's new is the 'let container =' preceding it. How about we examine that portion one word at a time.


# Sandbox

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

Unforunately, this won't work. Anytime you get a box off the shelf and label it, Swift needs to know what type of thing it's able to hold. By giving 'myBox' an initial value of 20, you're telling Swift that this box is meant to hold Ints. That means that when you try to put a String into 'myBox' on the next line, Swift is going to reject the attempt. You can think of it as trying to put an airplane into a box meant for a bicycle--the most obvious difference between these two types is in size, but there are other differences as well, and every single difference matters when it comes to putting one into a box meant for the other.
