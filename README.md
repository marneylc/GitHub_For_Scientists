GitHub_For_Scientists
=============================

Introduction to using Git and GitHub for scientists
----------------------------------------

Git is a version control system, read more about it here: http://git-scm.com/ . We are using Git as a flexible tool to handle the complicatedness that comes from having many scientists using code to processing chemical data, while at the same time other scientist are modifying the source code. If you don't really care all that much about code development, that is okay. If you use the source code, we are asking you to keep in mind the underlying process of instrument maintanance and software development and communicate your own expertise in a way that helps us organize and streamline our process with adequate documentation so that newer, better, and more flexible tools are available to you.

The first thing that I should say to help you form an idea of what this resource offers, is that Git and GitHub are two seperate tools that were made to work together. By this, I mean Git is a version control tool that you download to your computer for the purpose of organizing and maintaining your various source code projects. GitHub on the other hand is a web tool that syncs online repositories, like this one, with the code that you are using Git to locally manage. Through an intuitive branching structure, you can pull data from the online GitHub repository onto your computer where Git will help you manage the task of tracking the different iterations you may develope of that code. You can then push what pieces of your code you think are important from your local Git repository back into GitHub for the rest of the world to benefit from.

To futher clarify about GitHub, it is a website( https://github.com ) that has been optimized for the storing, sharing, and merging many separate Git repositories of descrete users, all via using the internet. If you have ever downloaded a file from the internet, you also have the  prerequisite skills to start using GitHub. To help you move beyond the basics, we offer help files in this repository that show where and how to acquire material already available to software enginners, but tailored to the scientist.

My job as owner/admin is to provide a stable organized file system that can be easily evaluated and developed without requiring you to learn a dozen new coding or administrative systems. Git and GitHub allow anyone (with the predefined access) to hack away at the fundamental source code whithout having to constantly ask for my permission first. So please, hack away! You don't need to know all that much about software engineering; as things like documentation, sources, and example data/figures are essential to good scientific documentation already, so by simply applying that lense to these resources you can help us improve the readability and applicability of this repositories contents.

At first, all you will need to learn is how to pull down the source code from the internet and run it on your local machine. As you get more comfortable, and start to make changes to your own copy of the code, such ass adding documentation and figures or links to example data, you may think that some of the changes you have made could be included in the source code. This is our true goal in providing such a robust open source repository. So when you inevitably do create something that you find to be more user friendly or applicable to your particular needs; Git and GitHub will make sharing that new tool with this repository and the rest of the world an easy, uncomplicated task.

Installation of Git
-------------------

Lets set up Git.

On windows, go here: http://git-scm.com/ and download the latest version of git for your operating system. Use the installer to get everything up and running. On debian based linux you can just type the following in a terminal.

``` shell
sudo apt-get install git
```

On mac, you can get git from http://git-scm.com/ or install it by brew
``` shell
brew install git
```

Configure Git
-------------

The nerdiest way to set up git to run is to open up *Git Bash* and set up your user name and email for Git:
``` git
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

If you plan on joining the company of nerds in changing this code, be sure to set the default text editor to an easy to use terminal text editor. The default is Vi, which is an awesome text editor, but has quite a learning curve. I recommend setting the default to nano and then you can learn Vi if you would like and set it back.

``` git
git config --global core.editor nano
```
