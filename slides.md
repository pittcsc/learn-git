# Version Control and Collaboration

> A primer on working smarter and enabling collaboration through a VCS

By Alex LaFroscia

---

# People are bad at coding

Note: If you think about it, we do stupid things all the time

----

- "Fixed" some code, messed it up, and need to undo everything
- Deleted an important file and can't recover it
- Moved some code while refactoring and can't remember what it was
- Commented out code to remember it because you'll need it eventually
- Wrote something a long time ago and forgot why

Note: All of these thing suck, or make our code messy

----

# You Need Version Control

----

## Two Simple Actions

- Save snapshots of your project
- Restore to any given snapshot

Note: These two simple actions enable us to avoid all of the problems that we just looked at

----

- Easy rewind to the last working version
- Recover a file from a previous snapshot
- View previous snapshots to reference old versions
- Leave yourself notes and details outside of the code itself

----

## So many flavors!

- Wikipedia lists over 40 types of VCSs, Git is just one
- Git has been made popular in part thanks to Github and open-source code
- You don't have to use Git, but please use something!

---

# Collaboration

Note: Many version control system have well-defined ways for sharing code between multiple developers.  Basically, this allows you to sync the snapshots that you have on your computer with those that other people have to make sure that everyone has the same code

----

![Github](http://www.molecularecologist.com/wp-content/uploads/2013/11/github-logo.jpg)

- Store code online
- Enables easy collaboration
- Find open source projects

----

# Open Source

- Tons of code available for use and learning, for free
- Big companies publish their code for other people to benefit from
- Anyone can contribute to any open source code

---

# How do I do it?

----

## Workshop on Wednesday, September 13th, 2017

7:00pm, Sennott Square Rm. 5317


---

# More Resources

- [https://help.github.com](help.github.com)
- [https://try.github.io](try.github.io)

---

# Git Workshop

---

# Tonight's Goal

----

1. Get Git installed and set up on our computers
2. Understand and use the basic commands of Git
3. Walk through the workflow of collaboration through Github

----

## Agenda

- Go over some Git vocabulary and commands
- Install Git, make Github accounts and set up authentication
- Practice using Git, including working with a shared repository

---

# Vocab

----

# Repository

- A project being organized by Git

----

# Commit

- High level: A "snapshot" of your project
- Low level: A record of changes since the last commit
- Each has a unique identifier, called a *hash*
- Contains information about what was added

----

# Branch

- A collection of commits
- *master* is the main branch
- *branch off* from master and *merge* back in

----

![branch-diagram](http://4.bp.blogspot.com/-s2F8W3gotyA/UAhePAGYO7I/AAAAAAAACeY/1SzXhEd7flk/s1600/theirsmerge-during.png)

----

# Remote

- A server that stores a copy of your repository
- Used to save your work off-site and enable collaboration
- You *push* to a server and *pull* from a server

---

# Commands

----

# `git status`

> Check the current status of your project

```bash
$ git status
On branch workshop-slides
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

    modified:   slides.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

    test-file.txt
```

----

# `git add`

> *Stage* a set of changes to be part of the next commit

```bash
$ git add test-file.txt // Stage one file
$ git add -A // Stage all of the current changes
```

----

# `git commit`

> Make a new commit

```bash
$ git commit // Will open your editor to write message
$ git commit -m 'My commit message!' // Make commit with messge
```

----

# `git push` and `pull`

> Push to and pull from a remote

```bash
$ git push origin master
$ git pull origin master
```

---

# Now it's your turn!

> http://github.com/pitt-csc/learn-git/wiki

If there are any questions or problems, come see me!
