Create your own repository
-------------------------

So you want to make your own repository and use it to store some info!

There are only a few commands you need to know. First we need make sure 
everything is how we want it with Git, and then we can use GitHub to 
backup the repository in the cloud.

So make a directory and put some files in it. Be sure to name the 
directory with the same name you are going to use for it on GitHub. My 
repository is creatively called "newrepository".

We can make a directory, navigate to that directory, and make a READE.md 
file all in the git bash terminal. (The **touch** command lets us create 
an empty file.)


``` git
mkdir newrepository
cd newrepository
touch README.md
```

You can always just do this in your file manager, just be sure to use the 
**cd** command followed by the directory to navigate to. The **pwd** 
command lets you know where you are, and **ls** lets you know what files
are in your current directory.


Make sure you are in the "newrepository" directory (use pwd). To initiate 
a git repository, add all changes in that repository for commiting, and 
then commit the changes with a comment letting you know what you did:

``` git 
git init
git add *
git commit -m "My first commit"
```

We now have a Git repository on our local computer, but we would like to 
push this repository to GitHub. First go to GitHub in your web browser 
and create a new repository using the green "New" repository button. 
Be sure to name it with the same name as the directory you used 
(newrepository). 

Once you give it a name and create the repository, copy the url in the 
quick setup box and run the following command in Git Bash.

``` git
git remote add origin https://github.com/marneylc/newrepository.git
git push origin master
```

Use your login credentials to push your new repository to GitHub and 
then refresh the repository webpage and you should see your files.

Then you basically only need three commands for all further simple code 
development:

```git
git add <filename> # or you could use * to add all files
git commit -m "A simple informative message"
git push origin master
```
