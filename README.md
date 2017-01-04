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
Congratulations because you've just written code. It's true! The playground reads that _100_ you just wrote, and it evaluates it. Evaluating a line means simplifying it as much as possible by performing any and all operations on that line. In this case, there are no operations to perform--there's only the number _100_ that you wrote.

On the righthand side of the playground is a grey area that should at this point have _100_ printed in it, lined up with the _100_ you typed. This _100_ that you didn't type is the result of the playground's evaluating that line. And as we mentioned, because there are no operations on this line, it simply evaluates to _100_. And it works the same for any number you care to try. Whether you type _13_, _500_ or _10000_, you are writing code.

## Operations

Let's see how powerful this playground's evaluation can be. We'll start by trying some arithmetic. Type the following, one by one, into the playground:
```
90 + 90
4 * 8 - 10
120 / 4 + 6
```
After everything is entered, the first line should line up with a _180_ in the grey panel on the right side of the playground. In Swift, _\*_ means multiplication; therefore, the _4 * 8 - 10_ should line up with a _22_, as standard order of operation rules apply. Finally _120 / 4 + 6_ ought to line up with a _36_. Hopefully, you're starting to gain a better understanding of what evaluation means, and why these numbers and operators can be considered code.

## Variables

As you've seen, all the code you've written so far certainly gets evaluated. However, as of now the results of these evaluations are simply printed on the rightside of your playground, and then they disappear. Basically, by the time the next line is being evaluated, the previous line is history. So let's not forget our history (because otherwise, just as in the real world, we'd be doomed to repeat it). 

A way we can do that is by storing evaluation results in variables. A variable is like a container that you label so that you can come back to it, identify it and use whatever it holds inside. Let's see how you do this in code:
```
let myContainer = 90 + 90
```
The above line might look intimidating, but let's make it less so by starting with the part we already know. The _90 + 90_ should look familiar to you as it's one of the first lines of code we wrote together. As you may remember, when _90 + 90_ is the only text on the line, the program evaluates it to be _180_. In an identical fashion, the first thing the program does when it reads this line is to evaluate that _90 + 90_ as _180_ again. At this point, both you and the program can imagine the line as reading the following:
```
let myContainer = 180
```
Now let's tackle the new portion. The first word in that statement, __let__, is a keyword in Swift, and it is how you declare a variable. Whenever you see __let__, you can imagine going to the container warehouse and picking out a brand new container in which you're going to store something. 

The next word, _myContainer_, is the label you're giving to your new container. Unlike __let__, _myContainer_ is not a keyword, meaning you could have put almost any word in its place. You could have labeled the container _blue_, _alpha_ or even _desperateHousewives_. There are a few rules when it comes to labeling your containers--you can't use keywords like __let__ and you can't use special characters like spaces. You can have fun naming your variables, but your future self will probably thank you if your containers are labeled accurately and descriptively based on what they hold.

The final new piece is that __=__ sign right between _myContainer_ and _180_. The __=__ is how you tell Swift what should go inside your new container. One of the most important things to remember about the __=__ is that Swift evaluates everything to the right of it before it puts the result into the container. In other words, _myContainer_ doesn't care how _180_ was reached, it just knows that it now contains it.

The ultimate result of this line of code is that our work is no longer immediately forgotten. Unlike our first bit of code in which our line was evaluated and merely forgotten, this line's effects are longer lasting. The variable we created, _myContainer_, not only exists in all following lines of our playground, but it also holds that '180' for us and it won't ever forget it.
