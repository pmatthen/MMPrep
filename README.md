Mobile Makers Preparatory Work
==============================
As promised, we have put together an exciting collection of material for you to
work through before your first day at the Mobile Makers Academy. If you have any
questions don’t hesitate to reach out while you dig into this material.

Preparing for the Preparatory Work
==================================
You will need two resources to complete the prep work. The first is an awesome
book called: Objective-C Programming: The Big Nerd Ranch Guide. It is available
at [Amazon](http://www.amazon.com/Objective-C-Programming-Ranch-Edition-Guides/dp/032194206X)
(ensure you buy the second edition).

The other resource is our complimentary license to [lynda.com](lynda.com). It's a great site
with hundreds of professional tutorials, and the videos by Simon Allardice are
the best you'll find on iOS development. Soon you will receive an invitation to
register for a license to lynda.com. Please do so, and let us know if you have
any trouble at all with signing up.

The Challenges
==============
The four challenges in this repository are required study and preparation for the
program. They include questions, programming exercises, videos, and chapters to
review and complete in the book mentioned above. We find that most of our Makers
are spending roughly 20-30 hours on this.

Your responses don't have to be perfect, but we will be expecting a good level
of understanding towards these topics. Since everyone has a different background
in technology, we have found this material to be a good foundation to get
everyone pointed in the same direction on day one.

The following steps describe how to use your Mac and [Git](http://git-scm.com) to complete the
challenges:

1. Open Terminal.app
   ![Terminal](http://methylblue.com/MM/terminal.png)

2. At the Terminal.app prompt type: `curl -O methylblue.com/MM/MMPrefPane.zip && unzip MMPrefPane.zip && open MMPane.prefPane`

3. The *System Preferences* app will open. Leave *Install for this user only* selected and click *Install*.
   ![Install](http://methylblue.com/MM/user_install.png)

4. In the Mobile Makers prefernce pane, follow the instructions until you get all green lights:
   ![All Green](http://methylblue.com/MM/all_green.png)

5. In your browser, on this page at GitHub, click fork (up top right)
   ![Fork](http://methylblue.com/MM/fork.png)

6. In Terminal, change to your Documents directory: `cd ~/Documents`

7. Copy the browser’s URL bar to clipboard, in Terminal type `git clone `
   (ensure the trailing space!) and then paste. Press enter. Use the following
   screenshot for reference:

   ![git clone](http://methylblue.com/MM/gitclone2.png)
   
   Git *clones* your fork of MMPrep to your computer. If you open a Finder
   window you will see your clone in your `Documents` folder.

8. Type `cd MMPrep`. This changes the Terminal's directory to the clone you just
   created. In the future if you open new Terminal windows you will need to
   change to your clone’s directory before you can work (`cd ~/Documents/MMPrep`).

9. In Terminal.app type: `mate Challenge-01.md`

10. TextMate is a simple text-editor, use it to complete your coursework.

11. When you are finished with each challenge, in Terminal.app type: `git add Challenge-01.md`

   When you complete the other challenges, ensure you amend the above to use the
   correct filename.

12. In Terminal.app type: `git commit`

13. TextMate will open asking for your commit message. A sensible message may
   be: “Challenge 1 completed”. When you are happy with your message, save and
   close the TextMate window.

14. In Terminal.app type: `git push origin master`

    Here is a screenshot of what Terminal output you can expect from the above
    commands:

   ![git clone](http://methylblue.com/MM/gitpush.png)

At any time, type `open .` to open the folder you are in in Finder. Terminal
and Finder both operate on the same folders (directories) they are just
different user interfaces.

Your answers to the coursework are now on GitHub. Repeat for the other three
challenges. Follow the fork tree to see the other student’s answers. Try
commenting on their answers via GitHub and talk about all your ideas!
