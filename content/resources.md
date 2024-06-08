---
layout: page
title: "Resources"
---

This page has links to useful resources.

## Practice problems and exams

Review materials for Exam 1:

* [Exam 1 practice questions](/resources/exam1review), [Solutions](/resources/exam1review-solutions)
* [Midterm, Spring 2020](/resources/midterm-spring2020.pdf) (Questions 1–3), [Solution](/resources/midterm-spring2020-soln.pdf)
* [Exam 1, Fall 2021](/resources/exam01-fall2021.pdf), [Solution](/resources/exam01-fall2021-soln.pdf)

Review materials for Exam 2:

* [Exam 2 practice questions](/resources/exam2review), [Solutions](/resources/exam2review-solutions)
* [Midterm, Spring 2020](/resources/midterm-spring2020.pdf) (Question 4), [Solution](/resources/midterm-spring2020-soln.pdf)
* [Final exam, Spring 2020](/resources/final-spring2020.pdf) (Questions 1–3), [Solution](/resources/final-spring2020-soln.pdf)
* [Exam 2, Fall 2021](/resources/exam02-fall2021.pdf), [Solution](/resources/exam02-fall2021-soln.pdf)

Review materials for Exam 3:

* [Exam 3 practice questions](/resources/exam3review), [Solutions](/resources/exam3review-solutions)
* [Final exam, Fall 2019](/resources/final-fall2019.pdf) (Questions 4–5), [Solution](/resources/final-fall2019-soln.pdf)
* [Final exam, Spring 2020](/resources/final-spring2020.pdf) (Questions 4–5), [Solution](/resources/final-spring2020-soln.pdf)
* [Exam 3, Fall 2021](/resources/exam03-fall2021.pdf), [Solution](/resources/exam03-fall2021-soln.pdf)

## x86-64 assembly language exercises

* [Assembly language mini-exercises](https://jhucsf.github.io/spring2024/resources/assemblyMini.html)
* [Assembly language exercise](/resources/assembly), [solution](/resources/asmExerciseSoln.zip)
* [Assembly language exercise 2 (more challenging)](/resources/assembly2)

## x86-64 assembly programming resources

* [CSF Assembly Language Tips & Tricks](https://jhucsf.github.io/csfdocs/assembly-tips-v0.1.2.pdf)
  * This is a very comprehensive guide to x86-64 assembly language written by
    Max Hahn, focusing on issues that are important for CSF
* [Brown x64 cheat sheet](https://cs.brown.edu/courses/cs033/docs/guides/x64_cheatsheet.pdf)
* [Brown gdb cheat sheet](https://cs.brown.edu/courses/cs033/docs/guides/gdb.pdf)
* [CMU summary of gdb commands for x86-64](http://csapp.cs.cmu.edu/3e/docs/gdbnotes-x86-64.pdf)

## Style Guidelines
* The [style guidelines](/resources/style) state our coding style expectations.

# Software

This section covers the software you'll be using in working on programming assignments.

## Linux

For the programming assignments, you will need to use a recent x86-64 (64 bit) version of Linux.

**Important**: the code you submit is required to run correctly on Ubuntu 22.04, since
that is the version of Linux that we use in [Gradescope](https://www.gradescope.com/) autograders.

Here are some options for getting your development environment set up.

You can use the [CS ugrad machines](https://support.cs.jhu.edu/wiki/Linux_Clients_on_the_CS_Undergrad_Net)
to do your development work. The ugrad machines use a recent version of
[Fedora Linux](https://fedoraproject.org/). Correctly-written
code will work the same way on Fedora and Ubuntu.

You can install [Ubuntu 22.04](https://releases.ubuntu.com/22.04/) directly on your
computer.  This is a good option if you are comfortable installing operating systems
from installation media.

On Windows 10, you can use the [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10)
(WSL).  Once WSL is enabled, you can install Ubuntu 22.04 from the Microsoft Store.  Make sure that
you install the [tools](#tools) listed below.  Using WSL is an excellent option if you are
comfortable doing your development work inside a terminal session.

<!--
On MacOS and Windows, you can use virtual machine software such as [VirtualBox](https://www.virtualbox.org/)
to run Ubuntu 22.04 as a guest OS.  If you do a web search for "ubuntu 22.04 image for virtualbox"
you will find pre-made OS images that you can download.  (I can't directly vouch for any of these,
so be careful.)  You will likely need to enable hardware virtualization support in your computer's
BIOS to allow VirtualBox to run correctly.  We recommend dedicating a significant amount of RAM
(at least 4GB) to the virtual machine (this should be fine as long as your computer has at least
8 GB of RAM.)
-->

Note that if you are using an Apple Silicon-based (ARM) Mac computer,
then (as far as we know) there aren't any good
options for setting up a local development environment.  Virtualization won't work
in the case because the computer doesn't use an x86-64 CPU. However, using
[Visual Studio Code](https://code.visualstudio.com/) connected to an SSH
workspace which accesses your ugrad account is a good option.

## Valgrind

Code that relies on undefined behavior (such as expecting the value of an uninitialized variable to
be 0) could very well behave differently on the autograder than it does when you run it on your development
system. Make sure that you test your code using [valgrind](https://valgrind.org/) to make sure there
are no memory errors.

## Tools

Some of the tools you'll want to have are:

* gcc
* g++
* make
* ruby
* valgrind
* git

All of these are available by default on the Ugrad computers.

To install on an Ubuntu-based system:

```
sudo apt-get install gcc g++ make ruby valgrind git
```

You'll also want to install a text editor.  [Emacs](https://www.gnu.org/software/emacs/) and [Vim](https://www.vim.org/) are good options:

```
sudo apt-get install emacs vim
```

## Vim setup
[Tutorial](/resources/vim) on setting up Vim

## Using Git
[Github ssh authentication](/resources/github-ssh): How to use ssh to access
your private repositories on Github
