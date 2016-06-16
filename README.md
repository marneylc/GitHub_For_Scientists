GitHub_MRC-HNR_Best_Practices
=============================

Introduction to using Git and GitHub for scientists
----------------------------------------

Git is a version control system, read more about it here: http://git-scm.com/ . We are using Git as a flexible tool to handle the complicatedness that comes from having many scientists using code to processing chemical data, while at the same time other scientist are modifying the source code. If you don't really care all that much about code development, that is okay. If you use the source code, we are asking you to keep in mind the underlying process of software development and communicate your own expertise in a way that helps us organize and streamline our process so that newer, better, and more flexibly code can be released to you.

The basic unit of Git is the repository. It is a directory on your local computer that contains the files that come together to perform some sort of program. Using Git, the history of all changes to code and all different off-shoots from the main source code are easily documented and organized.

GitHub is a website, https://github.com, that has been optimized to store, share, and merge Git repositories using the internet. If you have ever downloaded a file from the internet, you can start to use GitHub. The help files in this repository are a modification of material already available to software enginners, but tailored to the scientist.

My job as owner/admin is to provide stable source code and let the code be easily evaluated and developed. Git and GitHub lets anyone (who has access) hack away at the fundamental source code, whithout asking my permission first! So hack away! And you don't really need to know all that much software engineering, things like documentation, papers, and example data or figures are essential to good scientific source code, so please submit them where ever you think they should be.

At first you will want to simply know how to pull down the source code from the internet and run it on your local machine. As you get more comfortable and start to make changes to your own copy of the code (even documentation and figures or links to example data), you may think that some of the changes you have made could be included in the source code. So then you would like to let us know that you have some changes that you want to submit. Git and GitHub makes this very easy.

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

Set up your user name and email for Git:
``` git
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

Then be sure to set the default text editor to an easy to use terminal text editor. The default is Vi, which is an awesome text editor, but has quite a learning curve. I recommend setting the default to nano and then you can learn Vi if you would like and set it back.

``` git
git config --global core.editor nano
```
