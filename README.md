---
tags: deploy, team, git, pull request, kids
languages: html, css
resources:
---

## Getting to Know You...

For our first class project, we will be creating a student directory with your very own student profile.

Fork and clone this project to get started. We'll walk through the code together as a class.


## Structure

The structure of this project looks something like this:

```text
├── README.md
├── css
│   ├── css style sheets
│   └── fonts
│       └── font files
├── img
│   ├── lots of images here
│   └── students
│       ├── student_name_background.jpg
│       ├── student_name_index.jpg
│       └── student_name_profile.jpg
├── index.html
├── js
│   └── javascipt files
└── students
    └── student_name.html
```

### Files you will need to alter:
* The only file you'll alter is `index.html`.

### Files you will need to add:
* Add three pictures to the `img/students` folder (they can be jpg or png files):
  * A background picture
  * A picture for the index page
  * A picture for the profile page
* Add one HTML file to the `students/` folder. Use the `student_name.html` for reference. In fact, feel free to copy as much of the HTML from `student_name.html` into the new file you've created (just don't rename / override that file, as that will cause you some git headaches).

## Getting Started

* [fork](https://help.github.com/articles/fork-a-repo) this repo then [clone](http://ironboard-curriculum-content.s3.amazonaws.com/web-development/deploy-on-day-1/clone.png)

Take a look at `index.html` and `students/student_name.html` in the browser. You can do this many ways but one is by opening finder and right clicking on index.html. Then click on "Open with" then the name of your favorite browser.

* In this new branch, make a new HTML file in the `students/` folder. The file name should be the name of the student you're creating the profile for. Use the file `student_name.html` to see an example of what a profile's HTML could look like.
  * For instance, we would create a file `zoe_perez.html` in the main `students` folder.

* Still in this branch you created, add the three photos detailed above to the `img/students` folder. The student you're writing the profile for may have to email you their desired pictures or send you links to them, etc.
  * For instance, we would add the pictures titled `zoe_perez_background.jpg`, `zoe_perez_index.jpg`, and `zoe_perez_profile.jpg` to the `students` folder that is inside the `img` folder.
  * File endings are case senstive. When adding an \<image\> tag, make sure that the image source is identical to the name of the image file.

* Once you've completed the profile, open up `index.html`. Use the prexisting template as a model and add a section for your fellow student.

#### Stage and Commit Changes

* Once you're happy with the profile you've created and the changes you've made to the index page, type [git status](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Checking-the-Status-of-Your-Files). The the file you've altered, index.html, should appear in the "Tracked Files" section and the files you've created should appear in the "Untracked Files" section.

* You'll want to [add](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Staging-Modified-Files) then [commit](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes) these changes with a message.

* If you type `git status`, you should see "nothing to commit, working directory clean". If you type `git remote -v`, it should display something like:

|remote | url                                                               |         |
|-------|-------------------------------------------------------------------|---------|
|origin |https://github.com/table-member's-github-name/deploy-on-day-1...git| (fetch) |
|origin |https://github.com/table-member's-github-name/deploy-on-day-1...git| (push)  |

#### Push Up Your Branch

* Now it's time to [push](http://git-scm.com/book/en/Git-Basics-Working-with-Remotes#Pushing-to-Your-Remotes) to a remote branch. This remote branch doesn't exist yet, you're going to create it by pushing.
  * **NOTE: Do not push to master. Do not type anything that contains the word master!**
  * You're going to push to a branch that is the same name as your local branch.
    * For instance, if we're on the branch zoe-perez, we're going to push to zoe-perez.

* To confirm this push worked you can do two things:
  * Type ```git branch -a``` which will show the remote branch on github.com you just created when you pushed.
  * You could also go to the url of the forked repo. Notice the section that looks like ![branches](http://ironboard-curriculum-content.s3.amazonaws.com/web-development/deploy-on-day-1/branches.png). You should be able to click on that arrow and to see a dropdown. From this dropdown, select the name of the branch you've been working on.

## Final Steps

It's time to submit a pull request on the original repo.

* The first step is to go to the forked repo on your account.
* From this new view, click on ![pull request](http://ironboard-curriculum-content.s3.amazonaws.com/web-development/deploy-on-day-1/pull-request.png) on the right-hand menu. The green button with two arrows that looks like this ![green pull request](http://ironboard-curriculum-content.s3.amazonaws.com/web-development/deploy-on-day-1/green-button.png) will also work.
* On this new page, click the green button that says "New pull request". This will take you to a form.
Fill out the form and click "Submit".

Congratulations, you've completed your first assignment!

## Resources

* Git Step Resources
  * [Forking a Repo](https://help.github.com/articles/fork-a-repo)
  * [Cloning a Repo](http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository#Cloning-an-Existing-Repository)
  * [Branching](http://git-scm.com/book/en/Git-Branching-Basic-Branching-and-Merging#Basic-Branching)
  * [Adding](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Staging-Modified-Files)
  * [Committing Changes](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Committing-Your-Changes)
  * [Pushing to Remote Branches](http://git-scm.com/book/en/Git-Basics-Working-with-Remotes#Pushing-to-Your-Remotes)
  * [Merging Branches](http://git-scm.com/book/en/Git-Branching-Basic-Branching-and-Merging#Basic-Merging)
  * [Submitting a Pull Request](https://help.github.com/articles/using-pull-requests#sending-the-pull-request)
* Git Workflow Resources
  * [GitHub Flow](http://scottchacon.com/2011/08/31/github-flow.html)
  * [Git Workflow](https://github.com/diaspora/diaspora/wiki/Git-Workflow)
  * [Git Rebase Workflow Explained](http://mettadore.com/analysis/a-simple-git-rebase-workflow-explained/)
  * [How GitHub uses GitHub to Build GitHub](http://zachholman.com/talk/how-github-uses-github-to-build-github)
  * [GitHub Workflow for Submitting Pull Requests](https://openshift.redhat.com/community/wiki/github-workflow-for-submitting-pull-requests)

## Issues

A common issue is not being able to authenticate with GitHub. You need to use HTTPS/SSH correctly when cloning the repository in order to be authenticated with GitHub. Checkout and follow:

* [Setting Up Git](https://help.github.com/articles/set-up-git)
* [HTTPS Cloning Errors](https://help.github.com/articles/https-cloning-errors)
* [Setting Up SSH](https://help.github.com/articles/generating-ssh-keys)

