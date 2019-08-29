# BASH Overview

## Learning Goals

+ Identify differences between command-line interface, terminal emulator, and shell
+ Identify our "home directory" and how our file system is organized
+ Define "Command Line Interface" and describe why it's important
+ Use some common commands to navigate a computer's filesystem

## Outline

+ Hey folks, it's <NAME> from Flatiron School. In this video we're going to look at using the command line to create applications.
+ So our learning goals for this video are:
+ To identify the differences between command line interface, terminal emulator and shell.
+ Identify our home directory and how our file system is organized
+ To define command line interface and describe why it's important.
+ And to use some common commands to navigate a computer's file system.
+ So to start, let's talk a little bit about the history of computers. So way back when, in the 1980s, using a terminal was the only way to interact with computers. I'm going to Google 1980s terminal.
+ And computers have something like this.
+ With a monitor keyboard and the monitor would just output text. There was no mouse, you just sort of had to type in commands. And you'd see some text based output after typing the command.  
+ This was the only way back then to interact with a computer at all.
+ Today, the way that most of us use a computer is using the graphical user interface or a GU
+ Fun fact: the GUI and mouse were actually developed by the Xerox corporation at their research lab called Xerox Parc, but debuted to the public by Apple. If you're interested in the history, there's a great clip in the movie "Pirates of Silicon Valley". I'll include a link in the description.
+ Anyway, I'm using a Mac right now and the Finder is an example of this graphical user interface.
+ I can use my mouse to move my cursor around. I can click and see different folders. I can double click on applications like the Chess application and open this up and so I get this whole sort of graphical user interface to be able to to work with.
+ So this is one way using computer, but it's not the only way
+ We can still get a terminal interface for our computer, we can still get a text based representation
+ And there are reasons why developers might want to do that. It's faster to use.
+ It's easier to create tools and libraries if you don't have to worry about visual design or how things look
+ So here on my Mac. I have a terminal emulator. And I can open up that application. It's actually the utilities folder.
+ And that's going to open up right here.
+ So whenever I talk about a terminal going forward. This is what I'm going to talk about.
+  This is what I'm referring to an application that I can open up that I'll be able to type commands into you and it'll give me some output as if I was using one of these old terminal machines.
+ Every time I open a terminal I launched something called a shell. The shells job is to take commands from the terminal and communicate with the CPU or the central processor to actually like run those instructions.
+ So I'm using a shell called Bash, which is a really popular one that comes with Mac and Linux machines. There other shells that you try to use, but this is the one that we're going to use for the duration of this course.
+ So this is my terminal. And when we say command line interface or CLI we are just talking about any program that we run from our terminal. So we'll learn both to use CLI applications and I to write our own applications during this course.
+ If you're using the Learn IDE. We actually have a terminal emulator built in right here. So up here in the Learn IDE sandbox. I can see my text editor. This is where I could type code. And down here is my terminal emulator. This is where I can actually like read my applications.
+ So let's take a look now and a few basic bash commands that we will use every day in our careers developers.
+ I'm using the Learn IDE , which includes a terminal interface that I can use this is actually running in my web browser and being processed on a remote server somewhere, but it'll emulate what a typical terminal might look like.
+ The first thing I might want to do is remember that our computer is using that directory structure.
+ The graphical user interface way of representing this is by folder. So I have a utilities folder that has some
+ Applications in it, and it also has another folder here with some other applications in it.
+ And when I'm using the terminal emulator. We still have that directory structure. So you could picture just a series of folders inside of each other.
+ Sometimes you might want to say, hey, what's the home directory. What's sort of the main folder for that.
+ That's going to be represented on the terminal buys the tilda character. My tilda key on my keyboard is in the upper left hand corner right next to the one and I have to press shifts to access it.
+ So that kind of represents my home folder. If I wanted to know what folder I'm in right now, I want to say print working directory or PWD
+ And I can see here I'm in the home folder and then a folder called HOME name and then a folder called development. So that's my current directory
+ Now, maybe there are other files or folders here in this directory. And if I want to list all of those out. I can say ls for list.
+ Right now,  we just have this Readme file in here that's the one that's that's in there right now.
+ Sometimes you might want to move around to different directories. I can say CD, for change directory. dot.dot.is done moved me up one directory
+ And now I see that tilde - I can see I'm in my home folder right now.
+ I can say LS here.
+ And see that I have the development folder as well as a welcome file and some temporary files here.
+ So I'm going to CD back into my development folder.
+ And now I want to make a new file. That's actually something that you can't do in the Finder. There's no way for you to just make a new file, but using the terminal. I can do this really quickly by using the touch command
+ Awesome. So automatically, here we see that that popped up. I can also see this by doing an LS and see that we have my new file right there, which is great.
+ I can also make a new directory usually mkdir.
+ I'll make a new directory call new-stuff - using dashes instead of underscroes for folder names, to look a little bit nicer
+ Cool, I can see that new directory now.
+ I can move files around using the command called MV
+ so mv new_file.rb new-stuff will move the file into that directory. Fun fact: you can also use mv to rename a file - since you're really moving a file from one name to another.
+ Cool. And so if I do an ls now while I just see this new directory and said, I want to list out everything that's in that new directory
+ Two ways I might do that. I could cd into the new directory or if I want to quickly look without changing I might just say LS
+ new-stuff and that'll tell me everything that's in that directory
+ Finally, the last kind of common thing that you might want to do is to actually remove a file or a folder, and this is something that you want to be really careful with
+ This cannot be un-done. And if I'm not careful, I could actually delete my whole hard drive. When I do this. So I don't want to kind of double check before I remove that this is something that I actually wanted to do. But in this case, let's go ahead and remove that new file. So I'm going to see into the future.
+ I'm going to remove that file by saying our new underscore files off hard be and one little shortcut. If I start typing this out and press the Tab key.
+ The my emulator will actually predict what I'm trying to do and watch a finished that command for me so I can save myself a lot of typing but just starting to take what I say impressive stat.
+ Cool. So I remove that file. And as you can see, it didn't say anything. It didn't give me any output. But if I do an ls now.
+ I can see that there's nothing in here. So that's something kind of common with a lot of these terminal commands, is that there's no news is good news. If it didn't complain. It probably did the thing you want to do.
+ I'm going to cd up one level using CD, dot, dot. And I also want to remove this directory
+ So I'm gonna say rm new-stuff.
+ And we can see I'm getting an error here. So remember no news is good news, but in this case I did get this it says cannot remove new there. It is a directory. So I can't use the arm file on its own.
+ To remove a directory and then I have to say are and that car.
+ Newsletter. And what that dash are says is, hey, do this in such a way that you'll also delete anything that's inside of that directory, too. So this is something I want to be extra careful with
+ And we really want to make sure that this is something that I want to do before I before I do it.
+ Cool. And now it's disappeared.
+ So we've covered a lot of ground in this video. Let's recap the learning goals.
+ We've talked about the difference between the command line interface a terminal emulator and a shell. So remember our shell is the thing that's taking our commands and translating them into some hidden CPU can understand. Our terminal emulator is right here and lets pretend like we're using a terminal from back in the day, and Command line interfaces are any program that runs from here in the command line.
+ For example, I can run a program called echo. And that's a print out whenever I type in there so we didn't see that. It just prints out. Hi.
+ We also identified our home directory from Tilda. This is especially important if you're using a local file system to know where your home directory is
+ And we looked at a bunch of different commands such as pwd, cd, ls, touch, mkdir, and rm and rm -r to navigate our file system.
+ Hopefully you feel a little bit more confident in using the command line now - thanks for watching! 
