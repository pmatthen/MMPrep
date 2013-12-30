From the Lynda.com video series “Foundations of Programming: Object-Oriented
Design”, watch each (short) video and answer the correlating questions:


Section 0: Introduction
=======================
[0.1] What to expect from this course (3:06)
--------------------------------------------
What is the intended purpose and potential advantage of learning object oriented
design?

**Learning Object Oriented Design, potentially leads to greater clarity in our code, and improves our ability to communicate it to others. While Object Orientated languages are not more powerful than procedural languages, they allow us to break a complicated program into simpler, more manageable parts.**

[0.2] Exploring object-oriented analysis, design, and development (1:41)
------------------------------------------------------------------------
Why might it be advantageous to analyze and design before beginning programming?

**The strategy of first, understanding the problem, and then making a plan on how to go about solving the problem, before actually building a solution to the problem, leads to a more efficient use of time and effort. This becomes more apparent, as the complexity of the problem being solved increases.**

[0.3] Reviewing software development methodologies (4:08)
---------------------------------------------------------
What is the difference between a "waterfall" and an "agile" approach to
development? What is an iteration and how do we to use them to build software?

**The waterfall approach is a strict linear plan with several distinct steps. Only after one step is completed would one move on to the next step. On the other hand, the agile approach has many iterations of analysis, design, programming that allow for a lack of clarity in the initial to mid stages of a project.

An iteration is a cycle. In terms of building software, it is a cycle of analysis, design, and programming. Due to bugs, changing requirements, and changing expectations from clients, it is not reasonable to expect a completely accurate analysis and design of the problem on it's initial attempt. Instead, to accommodate for the lack of clarity in the early to mid stages of a project, we employ the agile approach.**


Section 1: Core Concepts
========================
[1.1] Why we use object-orientation (2:42)
------------------------------------------
What are the various types of programming languages and in which domain is each
used?

**Logic programming languages (Academic)
Functional programming languages (Academic)
Object-Oriented programming languages (Practical)
Unix Shell Scripts (Data Organization)
ColdFusion Markup Language (Scripting for data-driven websites)
Erlang OTP (Telecom)
FilterMeister (Photoshop filters)
MediaWiki templates (Page Templates)
Metacompilers (compiler writing)
Unreal Engine (Games)
Business Rules Engines (Policy and Business Rules)
Jags (Statistical Modeling)**

[1.2] What is an object? (5:22)
-------------------------------
Describe in your own words the three properties of a computing object.

**Computing objects have three basic properties. The first is identity, if there are two mug objects, one can be full while the other can be empty, one can be black while the other can be white. The are similar yet different, they have their own identity.

The second property is Attributes. There are characteristics that describe the state of an object. These characteristics are known as attributes. Attributes can be static or variable.

The third property is behaviour. There are actions that an object can perform, or that can be performed upon an object. These actions comprise the behaviour of an object.**

[1.3] What is a class? (4:43)
-----------------------------
Explain how classes are analogous to blueprints. Include the relationship
between a class and an object. Can you think of how the analogy breaks down?

**In the same way blueprints are definitions that are used to build houses, classes are definitions that are used to build objects. Classes define what attributes an object can have, and what behaviour can be performed by and upon them. The analogy breaks down, because houses can deviate from their blueprints, but classes cannot.**

[1.4] What is abstraction? (2:45)
---------------------------------
When a developer uses the term “abstraction” what are they describing?

**An idea or concept of an object that is completely separate from any specific instance. It only focuses on the essentials specific to the application we are writing, and ignores the irrelevant and unimportant.**

[1.5] What is encapsulation? (3:45)
-----------------------------------
What does encapsulation prevent? What does it enable?

**Encapsulation prevents manipulation and examination of your objects attributes and behaviours, except through the defined methods. By doing this, it limits inter-dependencies between software components and makes the system less complex and more robust.**

[1.6] What is inheritance? (3:35)
---------------------------------
Describe the inheritance relationship between classes. When would this
relationship be advantageous to establish?

**Subclasses can define new attributes and behaviour while inheriting existing attributed and behaviour from a Superclass. This saves coding time and allows changes in a Superclass to be reflected in all of it's Subclasses.**

[1.7] What is polymorphism? (3:22)
----------------------------------
What is the basic idea behind polymorphism? How can it make the classes we
create more flexible?

**Different classes can have methods with the same name. And code can be written that will perform the correct class method depending on the class of object specified. Using polymorphism, we can write code not knowing which class of object will be specified.**


Section 2: Object-Oriented Analysis and Design
==============================================
[2.1] Understanding the object-oriented analysis and design processes (4:13)
----------------------------------------------------------------------------
What are the steps of analysis that come before writing code for an application?
Why do you think these steps make writing the code easier?

**1. Gather Requirements
2. Describe the Application
3. Identify the Main Objects
4. Describe the Interactions
5. Create a Class Diagram

By having an idea of what problem we are trying to solve, a description of what the application will do, we can identify the main objects the app will use. From there we can describe the interaction between the main objects. Finally we can create a class diagram, which can help us identify where inheritance and polymorphism may be used.

By following these 5 steps we will gain a better idea of how to build the application, before writing any code.**

[2.2] Defining requirements (6:09)
----------------------------------
What should you have after you've completed the first phase of defining your
requirements?

**The features of the app that are required in order for it to function as described. These will act as a sort of checklist that must be completed when completing the initial design phase of the application.**

[2.3] Introduction to the Unified Modeling Language (UML) (1:54)
----------------------------------------------------------------
What is UML? Why Is it useful to visualize your application before coding it?

**UML is a graphical notation, used to draw diagrams of an object oriented system.  It is useful to visualize our application before coding it, because it is easier to see the interactions between classes and it is also easier to communicate and discuss it amongst a team.**

Section 3: Utilizing Use Cases
==============================
[3.1] Understanding use cases (6:11)
------------------------------------
Write a use case for creating an event on your phone's calendar.

**Title: Make a new appointment
Actor: User
Scenario: 
1. User selects 'Make a new appointment' from the calendar application menu. 
2. User fills in the date of the appointment. 
3. User fills in the start and end time of the appointment. 
4. User fills in the category of the appointment. 
5. User requests a notification for the appointment and specifies how long before the appointments start time the notification will take place. 
6. The system checks whether there are any conflicts with the new appointment and notifies the user accordingly.**

[3.2] Identifying the actors (4:16)
-----------------------------------
Can you think of a use case for a mobile application in which the actor is not
the user of the mobile device?

**In a chess application, an actor may be an opponent that plays remotely or the mobile devices computer. Therefore the use case that outlines the opponents move would be an example.**

[3.3] Identifying the scenarios (5:07)
--------------------------------------
Write another use case for a mobile device user interacting with a calendar
application. This time include a couple extensions when crafting your scenario.

**Title: Make an Appointment
Actor: User
Scenario:
1. User selects 'Make an Appointment' from application menu.
2. User indicates date of appointment.
3. User indicated start and end time of appointment.
4. User fills in the category of the appointment. 
5. User requests a notification for the appointment and specifies how long before the appointments start time the notification will take place. 
6. The system checks for conflicts.

Extensions: New Appointment is at conflict with an existing appointment
	(a) User changes time of new appointment.
	(b) User changes time of existing appointment.
	(c) User lets conflict remain.
	(d) User cancels new appointment.**

[3.4] Diagramming use cases (4:18)
----------------------------------
Do a google image search for "use case diagram." Notice how many variations
there are. What do they all generally have in common?

**They have actors, and sometimes show inheritance from one actor to another. They also show use cases that are started by an actor or reflected upon an actor. Finally, it shows the interactions between actors through use cases.**

[3.5] Employing user stories (3:43)
-----------------------------------
Write 5 user stories to describe a mobile user interacting with his or her maps
application.

**1.
As a user
I want to activate my GPS 
so that I know where I am

2.
As a user
I want to search for a name of a business
so that I know its address

3.
As a user
I want to find the route to take between two addresses
so that I know how long it will take

4.
As a user
I want to see which restaurants are close to my location
so that I know where to go for lunch

5.
As a user 
I want to know how long it takes to the bus station
so that i know when to leave the house**


Section 4: Domain Modeling (Modeling the App)
=============================================
[4.1] Creating a conceptual model (1:59)
----------------------------------------
What’s your favorite color?

**Navy Blue**

[4.2] Identifying the classes (2:27)
------------------------------------
Identify the classes in the use case you constructed for a user interacting with
his or her calendar application in chapter 3.

**User
Calendar
Appointment
Notification**

[4.3] Identifying class relationships (2:38)
--------------------------------------------
Identify the relationships among the classes you found above. Create a
conceptual model where you diagram these relationships and then upload a picture
of your model below.

**ANSWER HERE**

[4.4] Identifying class responsibilities (6:43)
-----------------------------------------------
Identify the responsibilities of the classes you found above. List them here.

**User

Calendar
	- Reserve time
	- Check whether time is reserved

Appointment
	- Set start time
	- Set end time
	- Set category
	- Set Date
	- Notify user y/n?
	- Check conflict

Notification
	- Set time before appointment to notify
	- Set method of notification
	- Alert User**

[4.5] Using CRC cards (2:49)
----------------------------
If you’d like, try creating CRC cards for the model you made above. There's no
need to respond here, just try it out and see if you like this form of
organization.

**ANSWER HERE… IF YOU LIKE**


Section 5: Creating Classes
===========================
[5.1] Creating class diagrams (6:11)
------------------------------------
Construct Class Diagrams for the classes you imagine exist in a twitter app, a
maps app, a calendar app, or any other app you would like to make. Do you find
that it is easier to come up with the attributes or with the behaviors? Why do
you think that is?

**I find it easier to come up with the behaviors first, because they give me a better idea which classes should hold which attributes.**

[5.2] Converting class diagrams to code (4:57)
----------------------------------------------
How might the separation of interface and implementation in Objective-C be an
advantage when working with class diagrams?

**The interface file in Objective-C would contain something quite similar to a class diagram and thus be more easily comparable. This becomes more apparent as methods become more complex and longer.**

[5.3] Exploring object lifetime (5:55)
--------------------------------------
What are the constructors and destructors in Objective-C? Why do we use them?

**Constructors are methods that create a new instance of an object, and inputs the objects variables with meaningful values. They are often required in complex objects that create objects of their own.

Destructors are methods that are called when an object is no longer needed and is being disposed of. Destructor methods delete an object so that system resources are freed up, also any connections to files are severed as well.**

[5.4] Using static or shared members (5:22)
-------------------------------------------
Like the interest rate example in the video, give three additional examples of
data that would be the same for all instances of a class.

**1. Minimum Wage
2. USD to Euro Conversion Rate
3. Retirement Age**


Section 6: Inheritance and Composition
======================================
6.1 Identifying inheritance situations (6:49)
---------------------------------------------
Describe in your own words what inheritance is and how it is useful when
constructing classes.

**Inheritance occurs between a subclass and superclass. The subclass is a more specific type of the superclass. It will automatically have all the variables and methods contained in the superclass. Additional variables and methods can be added and existing methods can be overridden.

It is useful, because it can save the programmer time.**

[6.2] Using inheritance (2:43)
------------------------------
Referring to the apps on your phone, come up with three examples where you
believe methods are being inherited from superclasses and called by subclasses.

**1. In Garageband, their are a variety of keyboard instruments, that seem to be subclassed from generic keyboard instrument class, which in turn seems to be subclassed from a generic instrument class.

2. In Facebook, company pages and user pages seems to be subclasses of a generic page class.

3.  In Google Maps, there are different categories of addresses, such as addresses for public transport, addresses for businesses, and addresses for restaurants. These seem to be subclassed from a generic address class.**
