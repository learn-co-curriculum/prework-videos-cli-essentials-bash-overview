# BASH Overview

## Learning Goals

+ Identify differences between command-line interface, terminal emulator, and shell
+ View file contents with `cat` and `open`
+ Identify our "home directory"
+ Define "Command Line Interface"
+ Identify the current working directory" with `pwd` ("print working directory")
+ Navigate up one directory in the file system
+ Change directories using `cd`
+ List directory files in the shell with `ls`
+ Move or rename files and directories with `mv`
+ Create empty files with `touch`
+ Make new directories with `mkdir`
+ Remove files with `rm`
+ Describe the purpose of CLIs

## Outline
Cover basic directory structure, history of the terminal, and basic BASH commands (cd, ls, touch, mkdir)

**NOTE** No starter code require, simply open a Learn IDE in Browser Window to identify the terminal.

+ Discuss history of computers
  + "Way back when in the 1980s, using a Terminal was the only way to interact with computers."
  + Show Finder for Mac, how it's a representation of files that are on the computer. Graphical User Interface, or GUI
  + That GUI is one way to represent how our files are stored, but it's not the only way
  + Today, we can use Terminal Emulators to use our computers with a different, text-based representation.
  + Fun fact: The Graphical User Interface, Mouse, plus a bunch of other innovations were originally developed by Xerox at their research facility Xerox Parc. If you're curious why Xerox didn't turn into Apple, check out the movie Pirates of Silicon Valley. I'll link to this clip in the description.
+ Explain why software developers use terminal interface
  + It's faster to use
  + It's easier to create tools without a GUI. You don't have to worry about visual design, how things look, or how a user will access. You can simply let them download a small file, and they can run it directly from their terminal.
+ Describe CLI, Terminal Emulator, and Shell.
  + Open up a Terminal on a Mac. Describe: "Here on my Mac, we have a Terminal application. This is an app that let's use use a terminal interface. When we say "Terminal", this is the type of thing we're referring to.
  + Every time I open a Terminal, I launch something called a "Shell". The shell's job is to take commands from the terminal and communicate with the CPU to process them. I'm using a shell called BASH, which is a popular shell that comes with Mac and Linux machines. There are other shells you could use, but this is the one we'll use for this course.
  + When we say "Command Line Interface", or CLI, we're just talking about any program that we can run from our Terminal. We'll learn to both use and write our own programs like this during this course.
+ Demonstrate some basic BASH commands
  + Let's take a look now at a few basic BASH commands that we'll use every day in our careers as developers. I'm using the Learn IDE, which includes a terminal interface that I can use. This is actually running in my web browser and being processed on a remote server somewhere, but will emulate what a typical terminal might look like.
  + Demo the following commands:
  + pwd - what directory am I in?
  + ls (or ls .)- what's in this directory? . meaning current directory
  + cd .. - move up one directory
  + Discuss relative vs absolute paths
  + Create a new file with `touch`
    + this is something you can only really do from the Terminal
  + Create a new directory and move the file into that directory
  + Remove the file and the directory - warning, make sure this is what you want to do. This cannot be undone. Don't erase your own hard drive.
