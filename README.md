# TestingProj
Education on project structure

## Prerequisites

1. Install [Git](https://git-scm.com/downloads)

If you want you may install both, but if you have limited storage space feel free to choose one or the other.
Visual Studio Code is standard Coding Editor, whereas visual studio community is a full coding environment

Visual Studio Code is most popular to develop with.

2. Install [Visual Studio Code](https://code.visualstudio.com/Download)
   
   and/or
   
4. Install [Visual Studio Community](https://visualstudio.microsoft.com/downloads/)

## Getting Project on your computer

#### Downloading Project Locally

When you open Visual Studio Code, on the bottom right you are able to open a new terminal, or the keyboard shortcut is **ctrl + shift + `**

When you open Visual Studio, on the bar above click on view -> terminal, otherwise the keyboard shortcut **ctrl + `** should work

```
git clone https://github.com/CUNYHackKnight2025/TestingProj.git
```
Why do this: if you dont then you wont able to work on project on ur comp, alternative you can work on github codepsaces
What it does: git will make a request to the github server and make a copy of the latest project 

#### Moving branches

First lets understand branches

Each Branch is like a version of the project:
|- prod
|-- dev
|--- yourbranch

Finished code:
- Code that has been reviewed
- Code that has been tested

##### Production branch 

This branch is quite trivial, this is the branch that should be the least updated, this is where we hold the finished code.

##### Dev branch 

This is where we push finished code and test integration with the whole teams code. Here is where we want to see if our new code will break when combined with everyone elses

##### yourbranch

This is your personal branch that you create based off the dev branch. Wheter you are working on a small feature or a small bug fix this is where all the meat of the work is done.

Now lets move branches!

1. Move to dev
```
git checkout dev
```

2. Create a branch off dev
```
git checkout -b {type}/{Name}
```

Here is an actual example:

```
git checkout -b bugfix/checkbox
```

### Keeping your branch up to date in cross collaborative team

Occasionally, in a team setting dev branch will keep changing. You should always move to dev branch, git fetch and git pull.

What this does is gets the latest code in dev branch, which you can use to update the code in your branch. This makes sure that while you are building you arent missing stuff that may have already been built or stuff that can break your code.
