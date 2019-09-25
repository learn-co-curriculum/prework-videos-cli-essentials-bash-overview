# BASH Overview

## Learning Goals

+ Identify differences between command-line interface, terminal emulator, and shell
+ Identify our "home directory" and how our file system is organized
+ Use some common commands to navigate a computer's filesystem

## Outline

+ Hey folks, it's Ian from Flatiron School. In this video we're going to look at using the command line to create applications.
+ So our learning goals for this video are:
+ To identify the differences between command line interface, terminal emulator and shell.
+ Identify our home directory and how our file system is organized
+ And to use some common commands to navigate a computer's file system.
+ So to start, let's talk a little bit about the history of computers. In the very early days of computers, computers were actually split into pieces.
+ The mainframe - which did the actual computing, would be in a big room someplace. You as a human would interact with it using what was called a terminal.
+ A terminal was a mouse and keyboard where you could type in commands and see some output back.
+ So then, way back when in the 1980s, personal computers started becoming available for people to keep in their homes.
+ Still, the only way to interact with those computers was via a keyboard and monitor.
+ There was no mouse, you just sort of had to type in commands. And you'd see some text based output after typing the command.  
+ Today, the way that most of us use a computer is using the graphical user interface or a GUI
+ Anyway, I'm using a Mac right now this operating system is an example of a GUI.
+ Fun fact: the GUI and mouse were actually developed by the Xerox corporation at their research lab called Xerox Parc, but debuted to the public by Apple. If you're interested in the history, there's a great clip in the movie "Pirates of Silicon Valley". I'll include a link in the description.
+ I can use my mouse to move my cursor around. I can click and see different folders using the Finder. I can double click on applications like the Chess application and open this up and so I get this whole sort of graphical user interface to be able to to work with.
+ So this is fun, and a great way to use a computer, but it's not the only way
+ We can still get a terminal interface for our computer, we can still get a text based representation
+ And there are reasons why developers might want to do that. It's faster to use.
+ For another, it's easier to create tools and libraries if you don't have to worry about visual design or how things look
+ So here on my Mac. I have a terminal emulator.
+ Instead of being connected to a remote computer by a cable, your "terminal emulator" talks to the computer you're actually typing on.
+ I can open up that application. It's actually the utilities folder.
+ So whenever I talk about a terminal going forward. This is what I'm going to talk about.
+ Inside of my terminal, I can type commands and I'll see some output here as well.
+ Every time I open a terminal I launched something called a shell. The shells job is to take commands from the terminal and communicate with the CPU or the central processor to actually like run those instructions.
+ So I'm using a shell called Bash, which is a really popular one that comes with Mac and Linux machines. There are other shells that you can use, but this is the one that we're going to use for the duration of this course.
+ So this is my terminal. And when we say command line interface or CLI we are just talking about any program that we run from our terminal. So we'll learn both to use CLI applications and to write our own CLI applications during this course.
+ If you're using the Learn IDE - we actually have a terminal emulator built into it. So up here in the Learn IDE sandbox, I can see my text editor. This is where I could write some code. And down here is my terminal emulator.
+ So let's take a look now and a few basic bash commands that we will use every day in our careers developers.
+ The first thing I want to remember is that our computer is using that directory structure.
+ The graphical user interface way of representing this is by folders. So I have an applications folder that has some files in it, plus a Utilities folder inside of that, that has other files in it, and so on.
+ And when I'm using the terminal emulator. We still have that directory structure.
+ Any time I execute a command, I'm executing it inside of a directory. My terminal has a concept of my "working directory" - the one that I'm working in.
+ If I wanted to know what my working directory is, I want to say print working directory or PWD
+ And I can see here I'm in the home folder and then a folder called HOME name and then a folder called development. So that's my current directory
+ As we can see here, the terminal also has a concept of a home directory. That's the main directory for your specific user.
+ That's going to be represented in the terminal buy the tilda character. My tilda key on my keyboard is in the upper left hand corner right next to the one and I have to press shifts to access it.
+ So that kind of represents my home folder.
+ Now, maybe there are other files or folders here in this directory. And if I want to list all of those out, I can say ls for list.
+ Right now,  we just have this Readme file in here.
+ Sometimes you might want to move around to different directories. I can say CD, for change directory. `cd ..` is the shortcut to move me up one directory, or I can give it a different path, such as `cd ~` to go home.
+ And now I see that tilde - I can see I'm in my home folder right now.
+ I can say LS here, and see that I have the development folder as well as a welcome file and some temporary files here.
+ So I'm going to CD back into my development folder.
+ Let's learn now how to create new files. That's actually something that you can't do in the Finder. There's no way for you to just make a new file, but using the terminal, I can do this really easily by using the `touch` command
+ Awesome. So automatically, here we see that that popped up. I can also see this by doing an LS and see that we have my new file right there, which is great.
+ I can also make a new directory usually mkdir.
+ I'll make a new directory call new-stuff - using dashes instead of underscores for folder names, to look a little bit nicer
+ Cool, I can see that new directory now.
+ I can move files around using the command called MV
+ so mv new_file.rb new-stuff will move the file into that directory. Fun fact: you can also use mv to rename a file - since you're really moving a file from one name to another.
+ Cool. Say I want to list out everything that's in a different directory than the one I'm in.
+ There are two ways I might do that. I could cd into the new directory, or if I want to quickly look without changing I might just say `ls new-stuff` and that'll tell me everything that's in that directory
+ Finally, the last kind of common thing that you might want to do is to actually remove a file or a folder, and this is something that you want to be really careful with
+ This cannot be un-done. And if I'm not careful, I could actually delete my whole hard drive when I do this. So I want to double check before I remove that this is something that I actually wanted to do. But in this case, let's go ahead and remove that new file.
+ I can remove a file using the `rm` command followed by the file-name.
+ Cool. So I remove that file. And as you can see, it didn't say anything. It didn't give me any output.
+  But if I do an ls now, I can see that there's nothing in here. So that's something kind of common with a lot of these terminal commands, is that no news is good news. If it didn't complain. It probably did the thing you wanted it to do.
+ I'm going to cd up one level using `cd ..` And I also want to remove this directory
+ So I'm gonna say `rm new-stuff`.
+ And we can see I'm getting an error here. So remember no news is good news, but in this case I did get some news. This it says cannot remove this because it is a directory. So I can't use the `rm` command on its own for directories.
+ To remove a directory,  I'll add a flag to the `rm` command. Flags are like little modifiers that start with a `-`
+ In this case, I'll do `rm -r` - the `-r` flag says, when you remove that directory, also remove everything inside of it.
+ Fun fact: r stands for "recursive" here - recursion means the process of repeating something over and over.
+ So if I run `rm -r new-directory` - cool, we see that this worked.
+ So we've covered a lot of ground in this video. Let's recap the learning goals.
+ We've talked about the difference between the command line interface a terminal emulator and a shell. So remember our shell is the thing that's taking our commands and translating them into some hidden CPU can understand. Our terminal emulator is right here and lets pretend like we're using a terminal from back in the day, and Command line interfaces are any program that runs from here in the command line.
+ We also identified our home directory. This is especially important if you're using a local file system to know where your home directory is
+ And we looked at a bunch of different commands such as pwd, cd, ls, touch, mkdir, and rm and rm -r to navigate our file system.
+ Hopefully you feel a little bit more confident in using the command line now - thanks for watching, and happy coding! 
