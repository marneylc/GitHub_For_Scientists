Checking the parent MRC-HNR repository for updates
--------------------------------------------------

To get any changes from the parent repository we first need to add the parent repository to what git calls a "remote". For our purposes this simply means a pointer to a GitHub URL.

``` git
git remote add upstream <url>
# <url> is the url for the parent repository, 
# and will be in the form https://github.com/MRC-HNR/RepoName.git
```

Tell git to go get the "upstream remote", in our case this is the MRC-HNR parent repository in GitHub.

``` git
git fetch upstream
# in git language: grabs upstream remote's branches
```

You can now take a look at the changes we, the administrators, have made.

``` git
git diff --stat remotes/upstream/master master
# compares the two branches:
# 1) remotes/upstream/master <- which is the parent repository
# 2) master <- which is our own forked repository that was cloned onto the machine we are working on
```

If there are any insertions or deletions you can run the previous command without the "--stat" argument to see details about the specific differences between your local copy and the parent MRC-HNR repository. To merge your copy with the parent MRC-HNR repository:

``` git
git merge upstream/master
```

This will make any changes to your own repository currently on your computer (on currently active branch, which is the master branch). To have those changes added to your own GitHub fork, simply run:

``` git 
git push origin master
```

If you go look at your own GitHub repository you should see the changes added to it.
