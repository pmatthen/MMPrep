Challenge 3: Get Your Hands Dirty
=================================
Next up, find the Lynda.com video series entitled: “Objective-C Essential
Training”. Watch each video in the following list and answer the corresponding
question.

Section 1: Getting Started
==========================
[1.1] Installing the tools (4:42)
---------------------------------
You should already have Xcode installed, but you will need to register as an
Apple Developer.

Do you like cats?

**Not really**

[1.2] Creating your first application (11:28)
---------------------------------------------
Create your first application using the same steps Simon describes in the video.
Familiarize yourself with the Xcode environment, specifically notice how it can
be manipulated to display different helper tools and how it will attempt to fill
in your code as you type it.

**Yes**

[1.3] Updates to this course (3:31)
-----------------------------------
Why do you think it's important to be aware of the idiosyncracies with older
versions of Objective-C and to keep up with new features as they are added?

**It is important to be aware of the older versions of Objective-C, because it will reduce confusion while reading code written in the older versions. It is important to keep up with the new features, because they will generally make programming easier.**

Section 2: Objective-C Basics
=============================
[2.1] The Objective-C language (4:11)
-------------------------------------
How did Objective-C become the language to learn if you want to make apps for
the iPhone and iPad?

**Objective-C was the main language used by Next Computer, a company founded by Steve Jobs in 1985. Apple bought Next in 1996 and used Next Computers OS NextStep as a foundation for OSX, iOS was build on OSX, and thus also uses Objective-C.**

[2.2] The structure of an Objective-C program (6:15)
----------------------------------------------------
Create a new project. Go to the menu option `Xcode`, `Preferences`,
`Text Editing` and make sure *Line Numbers* is checked in the section marked
"Show." Then add comments describing the purpose of each auto-generated line in
the main.m file. For example on Line 17 I would write: 

```
NSLog(@"Hello, World!");  // instructs the console to output: Hello, World!
```

[2.3] Compiling and running your code (8:37)
--------------------------------------------
Why might you build in one version of iOS but deploy in an older version?

**If a significant number of users you are targeting still use an older version of iOS, then you will deploy in an older version, so that they will be able to run your application.**



Section 3: Program Flow
=======================
[3.1] Logging messages to the command line (6:07)
-------------------------------------------------
Following the example in the video, write a program that calculates and outputs
to the console the number of seconds in ten years. Copy and paste your code
here.

**      int secondsInAMinute = 60;
        int minutesInAnHour = 60;
        int hoursInADay = 24;
        int daysInAYear = 365;
        int yearsInTenYears = 10;
        
        int secondsInTenYears = secondsInAMinute * minutesInAnHour * hoursInADay * daysInAYear * yearsInTenYears;
        
        NSLog(@"There are %i number of seconds in ten years", secondsInTenYears);**

[3.2] Writing conditional code (7:01)
-------------------------------------
Using Objective-C, create an integer variable called "day" that represents the
days of the week. Write an if statement that checks whether "day" is a weekend
day. If the day is a weekend day then have your program print a message saying
"Have a nice weekend!" and if it's not, print a message saying "I hope you're
having a good week!"

**      int day = 6;
        
        if ( (day == 5) || (day == 6) ) {
            NSLog(@"Have a nice weekend!");
        } else {
            NSLog(@"I hope you're having a good week!");
        }**

[3.3] The switch statement (5:58)
---------------------------------
Create a variable called "hurricaneCategory" and a switch statement that prints
out a message describing a hurricane's category from 1-5.

**      int hurricaneCategory = 4;
        
        switch (hurricaneCategory) {
            case 1:
                NSLog(@"The hurricane is a category 1 hurricane.");
                break;
            case 2:
                NSLog(@"The hurricane is a category 2 hurricane.");
                break;
            case 3:
                NSLog(@"The hurricane is a category 3 hurricane.");
                break;
            case 4:
                NSLog(@"The hurricane is a category 4 hurricane.");
                break;
            case 5:
                NSLog(@"The hurricane is a category 5 hurricane.");
                break;
            default:
                NSLog(@"The hurricane is unprecedented.");
                break;
        }**

[3.4] Code snippets (5:15)
--------------------------
Grab a code snippet, indent it to match the indent of your project, then add
comments to it, then select the entire snippet you just modified and save it as
your own code snippet. Time yourself and record how many seconds it takes you to
do all this.

**IT TOOK ME [20] SECONDS**

[3.5] Operators and expressions (11:08)
---------------------------------------
List the 6 types of operators described in this video. Provide their name, a
description of their meaning, and the syntax you would use to execute them. What
code snippet does the ternary operator replace?

**arithmetic operators: consists of addition (+), subtraction (-), multiplication (*), and division (/). They will perform the respective arithmetic operation on the two values. Example, (6 * 7) would give you (42).

comparison operators: consists of equal to (==), greater than (>), less than (<), not equal to (!=), greater and equal to (>=), and less than and equal to (<=). They will compare two values and return a true or a false. Example, (6 > 7) would give you (false).

logical and / or: consists of logical and (&&), and logical or (||). The compare two statements and returns a true or a false. Example, ( (6 > 7) && (7 > 6) ) would give you (false).

modulus: Returns the remainder of the division between two integers. Example, (2003 % 4) would give you (3).

increment / decrement: consists of (++) and (--). If written as a prefix (++a), it would increment the value of a and then execute the rest of the line of code. if written as a suffix (a++), it would execute the line of code and then increment the value of a. Example, (++6) would give you (7).

ternary operators: evaluates a condition and outlines what to do if true or if false. Example, (6 > 7) ? (NSLog(@"condition is true") : NSLog(@"condition is false") would give you (@"condition is false").

The ternary operator replaces the if, then, else statement.**

[3.6] Loops (8:53)
------------------
Think of a scenario while using a mobile app that might require you to use a
"continue" statement in the middle of a loop.

**When searching through an address book to find whether a contact contains a string. If the contact does contain the string you would use the "continue" statement to stop that iteration of the loop and move to the determining whether the next contact contain the string.**

[3.7] Functions (10:16)
-----------------------
What is a function? What is a function prototype? What are the purposes of each?
What are the rules for when and how you can call a function?

**A function is a block of code that has a name, a return type, and input parameters. A function prototype is a statement that tells the compiler that a certain function exists, it is written the same way the first line of the function is written, the actual function will need to be fully written elsewhere in the code.

The purpose of a function is allow code to be reused. The purpose of a function prototype is to allow the implementation of a function to be written after the function is called.

Unless there is a function prototype, a function can only be called after its implentation is defined. If the function has been defined to have input parameters, then when it is called, input parameters must be given in the type that was specified.**


Section 4: Variables
====================
[4.1] Data types (7:06)
-----------------------
What are the primitive data types in Objective-C? Why did Apple add a set of
classes to handle other data types?

**They are: int, float, double, char, and BOOL. Apple added a set of classes for other common data types so that programmers wouldn’t have to write them each time they want to work with them.**

[4.2] Working with numbers (9:33)
---------------------------------
Make a table of Objective-C primitive data types. Add numeric data types and
their properties to this table.

**int				can store a positive or negative whole number (format token = %i)
float				can store a positive or negative number with a decimal place (format token = 				%f or %e)
double			same as float, but double the size.

modifiers			unsigned (only positive), short (half the size), long (double the size), long long 				(4 times the size)

char				can hold a single character from the ASCII character set (format token = %c)
BOOL			can hold ‘YES’ or ‘NO’ (format token = %i)**

[4.3] Working with characters (4:39)
------------------------------------
Add char and BOOL (the character data types) to your table created above.

**ANSWER ABOVE!**

[4.4] Variable scope (8:06)
---------------------------
Describe in your own words what the scope of a variable is in Objective-C

**The scope of a variable in Objective-C refers to where the variable exists and can be accessed. It is within the statement block it is defined. For example, a variable defined within a for loop will not exist outside of that loop. Global variables (those that are define outside of the main statement block and are also not within a function) are possible, but are considered bad programming where they can be avoided.**

[4.5] Enumerations (3:35)
-------------------------
What does the `enum` keyword allow you to do?

**It allow you to create your own variable type that has restricted values that you define. These values are actually integers.**

[4.6] Using typedef (2:17)
--------------------------
When would you define your own data type versus using an enum?

**So that you wouldn’t have to write enum each time you define a variable of that type.**

[4.7] Preprocessor directives (5:56)
------------------------------------
Describe the three common preprocessor directives, `#import`, `#define`, and
`#if DEBUG`. Come up with one example where you would use each.

**#import - will search for the file you specified and include it where you write the #import statement.

#define - will allow you to create a macro, where you specify the name of the macro and then define what the macro is. Wherever you write the name of the macro in your code, it will be replaced with the macros definition.

#if DEBUG - Whatever code is written between #if DEBUG and #endif will only be processed if you are compiling in ‘debug’ mode. If you compile in ‘release’ mode it will not be processed by the compiler.

#import would be used when importing framework such as the Foundation framework. 

#define would be used for constants that are too long to write, or constant that appear in numerous places (to change them you would only have to make the change in one place).

#if DEBUG would be used while in the midst of a project, where you may want to check values to ensure they are as they should be, or when you want to see where a mistake is being made. Upon release, this code would not be processed.**

[4.8] Working with strings (7:52)
---------------------------------
Define the same string using both NSString and C-style string syntax. Describe
the purpose behind each part of your definition.

**ANSWER In NSString-style syntax my string would be @“Hello”, defining a string object.
In C-style syntax my string would be “Hello”, defining a string literal.**


Section 5: Classes
==================
[5.1] Introduction to object orientation (7:36)
-----------------------------------------------
Create an encapsulated (including generalized attributes and behavior)
description of a `MobileMakersParticipant` class. Instantiate a single object
representing yourself as a member of this class.

**Yes**

[5.2] Using objects and pointers (6:38)
---------------------------------------
What is the pointer’s role in instantiating an object from a class? How is a
pointer different than a primitive?

**The pointer contains an address for where the object is located in the systems memory. A primitive variable contains data, while a pointer variable contains an address for where an object is located.**

[5.3] Messages and methods (6:44)
---------------------------------
What is the main difference between Objective-C’s messages and method calls in
other languages? How can this difference be seen as an advantage while
programming?

**The messages and method calls in Objective-C are within square brackets opposed to the dot syntax. Additionally, each and every parameter that is passed is named. This makes the code more readable and maintainable.**

[5.4] Using existing classes in the foundation framework (8:40)
---------------------------------------------------------------
What's the difference between a class method and an instance method?

**A class method is a behaviour that is generic to the class (such as the date and time right now), whereas an instance method is specific to an instance of the class (such as the date and time specified in the instance).**

Try typing "NSD..." into your code window. Use the autofill feature and select a
single class name that starts with those three letters. Once the name has been
auto-completed, use the handy shortcut (Option + click) and investigate the
class whose name just got printed to the screen. Examine the task list for this
class. Do this a few more times until you're familiar with the process, or until
you've exhausted your curiosity, whichever comes last.


Section 6: Memory Management
============================
[6.1] What's new with memory management? (1:45)
-----------------------------------------------
Let it soak in. No questions for this one.

**PHEW**

[6.2] Memory management in Objective-C (6:58)
---------------------------------------------
What is the relationship between a pointer to an object, a block of memory, and
the owning and releasing process. Can you come up with an analogy for this
relationship?

**A pointer stores the address of a block of memory where an object is stored. When you create an object and store the address it is located in a pointer variable, or assign a ‘pointer to an object’ to another pointer variable, you have ownership and are responsible for releasing.

This could be compared (albeit weakly) to reserving a table at a busy restaurant. When you no longer need the table and your reservation is still active, you are responsible for cancelling it so the restaurant can seat other customers.**

[6.3] Object creation (7:31)
----------------------------
What does the new method do when used to create an object instance of a class?
Why do we avoid using this method? How long is an object's lifetime?

**It allocated a block of memory and initialises a null object from the class you specified. We avoid using ‘new’, because we wouldn’t be able to take advantage of other, more versatile (init and it's varieties), ways to control the instantiation and initialisation an object.

An object lives either until it is released (to a retain count of 0) or till the end of the program.**

[6.4] Using autorelease pools (5:14)
------------------------------------
How does the autorelease pool work? How and when can you use it deliberately?

**It reduces a variable called ‘retain’ (that is associated with blocks of memory) by 1. When the value of ‘retain’ is 0, the system knows that the block of memory can be written over.

We release objects that we have created or have been created on our request (using alloc or new, or retain or copy) once we are finished using them.**

[6.5] Apple autoreleased objects (3:39)
---------------------------------------
What does NARC stand for? Why is it important to remember this?

**N.A.R.C stands for New, Assign, Retain, Copy. It is important to remember, because we should release objects created using these terms. Objects that have been created without the use of these terms, should not be released by us.**

[6.6] Introduction to Automatic Reference Counting (ARC) (4:43)
---------------------------------------------------------------
What does ARC save us from having to do? How does it keep us from having to make
this extra effort?

**ARC saves us from having to release objects, by doing it for us. It does this using the LLVM compiler. The LLVM compiler goes through the code you have written and determines when the best place to release objects should occur.**

[6.7] What ARC manages (2:42)
-----------------------------
What are the differences between ARC and garbage collection? What makes these
differences advantageous?

**While ARC and Garbage Collection both automate memory management, they are different.  ARC analyses your code at compile time and optimally determines when objects should be released. It then adds these release statements to your code.

With Garbage Collection, there is a module that is constantly running that monitors memory usage of an application. When too much memory is being taken up, it jumps in to clean up. You cannot know when this will happen, and it can lead to slowdowns when memory is being reclaimed.

Using ARC allows your applications to have more processing power available to it. Additionally they do not experience slow downs at unexpected moments. **

[6.8] The rules of ARC (4:20)
-----------------------------
Why can you not release or dealloc memory when working with ARC?

**ARC does this work for you, so you are not allowed to use these statements, Xcode will give you an error.**


Section 7: Custom Classes
=========================
[7.1] Creating your own classes (14:01)
---------------------------------------
What are the two different sections used to create a class? What do they hold
and what files are they placed in?

**The two different sections are the interface section (stored in the .h file) and the implantation section (stored in the .m file). The interface section holds the names of the instance variables of the class as well as the method names and the parameters they require. The implementation file has the actual code that makes up the classes methods.**
    
**Challenge!** Create a Tweet class for a twitter style app.

[7.2] Defining methods (8:36)
-----------------------------
**Challenge!** Define what should get passed in and what should get returned by
each of your methods in your Tweet class above.

**Haven't gotten into it**

[7.3] Defining properties (7:21)
--------------------------------
How did Objective-C programmers handle instance variables before 2012? How are
they handled now? What got easier and what got obscured?

**Previously, they were grouped together inside a set of curly braces in your interface file. If you needed to ‘get’ or ‘set’ a variable from outside the class, you would have to write setter and getter methods for the variable. Now, each variable in the interface file is preceded with an “@property”, we no longer even have to generate setter and getter methods using the “@synthesize” keyword, that is now done automatically.

Now, a lot of code is assumed and generated for us, while this makes it easier for us, it also means that a lot of behaviour is hidden.**

[7.4] Defining initializers (12:30)
-----------------------------------
What are initializers and why do we need to use them? Describe a situations when
you can rely on the standard `init` method and when you have to create your own
custom initializer.

**Initialisers are statements that set the initial values of an object. We need to use them to make sure new objects are created in a valid state.

The standard init method will set all initial values to zero. Objects where initial zero values are wanted or objects that accept outside input to determine the values of the variables are correct situations for standard init methods. However, objects that have variables that should start at non-zero values can have custom initialisers.**

[7.5] Using dealloc (5:33)
--------------------------
Why can we have a dealloc method in a class when using ARC, but we can't call
dealloc manually oursevles when using ARC?

**We can have dealloc method in our classes when using ARC, because we sometimes need to close connections to resources that are not closed when destroying an object (such as a connection to a database). However, we cannot call dealloc manually, because ARC does this automatically and forbids these calls.**


Section 8: Collections
======================
[8.1] Working with C-style arrays (7:12)
----------------------------------------
What are the three constraints when using C-style arrays? Create a C-style array
that holds the days of the week.

**1. No bounds checking.
2. Fixed size
3. Can’t mix types.

NSString *daysOfTheWeekArray[7] = {@“Monday”,@“Tuesday”,@“Wednesday”,@“Thursday”,@“Friday”,@“Saturday”,@“Sunday”};**

[8.2] Working with Objective-C array objects (8:00)
---------------------------------------------------
What is the difference between a mutable and an immutable array?

**Once you create an immutable array, you cannot add objects to it or remove objects from it, it is a fixed size. Whereas you can add and remove objects from a mutable array**

**Challenge!**
Create an immutable array containing the days of the week. Create a mutable
array that contains the days of the week that you will be at Mobile Makers. Add
the days of the week from the immutable array to the mutable array.

[8.3] Using dictionaries (5:55)
-------------------------------
Create a dictionary that lists five or more events in your life and the
accompanying year (or date if you want to get fancy) of the event.

**Done**

[8.4] Fast enumeration (3:27)
-----------------------------
Use fast enumeration to log the timeline of the life events you described above
to the console.

**AYE AYE CAPTAIN**

Section 9: File Management
==========================
[9.1] Introduction to file management in Objective-C (6:44)
-----------------------------------------------------------
What can you do with files using the methods you are aware of that are available
in Objective C’s Foundation class?

**fileExistsAtPath - Checks whether the file exists at the path you specify.
attributesOfItemAtPath - Returns an NSDictionary object that is filled with attributes of the file whose path you specify.
moveItemAtPath - moves a file, whose path you specify, to the path you specify.**

[9.2] Working with paths and URLs (7:17)
----------------------------------------
What are the three parts of a URL? What are the advantages to using NSURL?

**They are the scheme, the domain , and the path. The advantages are that using NSURL is quicker (as snow leopard is optimised for them), it can trap errors (it will not accept URL’s that are not properly formed), and it is more powerful (as more classes utilise NSURL’s).**

[9.3] Reading and writing strings (4:38)
----------------------------------------
What would be a reason you would want to write a string to disk instead of just
keeping it memory?

**In order to keep a record of that string even after the program finishes running.**

[9.4] Archiving objects (12:41)
-------------------------------
Why would you want to archive an object instead of writing the data to disk
using the techniques discussed previously?

**I would prefer to archive an object, because the process would be simpler. Instead of writing methods to break apart the object and save different pieces to different files (and then writing to methods to reverse the process), I could take advantage of the NSKeyedArchiver and NSKeyedUnArchiver, and NSCoder. This would accomplish the same things, but be much simpler as these classes have already been written for me.**

Section 10 - More Complex Classes
=================================
[10.1] Inheritance and NSObject (8:13)
--------------------------------------
How can you determine what methods you're inheriting from a super class? How do
you overide a method inherited from a super class?

**You can find out the available methods of a class by taking a look at it’s class reference. You override a method inherited from the super class by providing your own version of it, it will need to have the same signature. You do not need to include the overridden method description in the header file.**

[10.2] Extending classes with categories (6:31)
-----------------------------------------------
What is the difference between a category and an inheritance? What are the
limitations of using a category?

**A category adds new functionality to an existing class, while inheritance allows you to use the functionality in an existing class and add new instance variables and functionality to it in a new class. You cannot add new instance variable to a category, making it more limited than a subclass.**

[10.3] Defining protocols (5:14)
--------------------------------
How are protocols useful?

**Certain classes require you to interact with them using certain methods. These methods (and their signatures) are defined in the classes protocol reference. Therefore, protocols guide you in writing these methods.**

[10.4] Dynamic typing (11:33)
-----------------------------
What are the advantages and disadvantages to dynamic typing?

**The advantage is that dynamic typing allows you to work with objects that are unknown. However, certain errors in your code (such as calling a method that does not exist) will not get recognised at compile time, instead they will cause your program to crash at runtime.**