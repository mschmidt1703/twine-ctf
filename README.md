# Memory Loss: Find Your Way Back
![](title.png)

This game was developed on the Twine engine to teach some basic knowledge about IT security and vulnerabilities using CTFs.

# Table of contents
1. [Memory Loss: Find Your Way Back](#memory-loss-find-your-way-back)
    1. [Overview of CTFs](#overview-of-ctfs)
    2. [How to start the Game](#how-to-start-the-game)
2. [Development](#development)
    1. [Requirements](#requirements)
    2. [Workflow](#workflow)
    3. [Git for Noobies](#git-for-noobies)
3. [Image Sources](#image-sources)
3. [Credits](#credits)

## Overview of CTFs
- XSS
- Web

## How to start the Game
1. Clone the repository
2. Change into /out
3. Double click to start the story.html

# Development
Everything you need to work with this project.

## Requirements
- Twine with Harlow 3.3.1
- Tweego

## Workflow 
1.) Pull the current data from repository:
```sh
git pull
```

2.) Build your local twine project to work on in 
```sh
tweego.exe src/ -o out/story.html
```
/src will always contain the current files.

3.) Import story.html in your twine folder. If work is done then export html file from Twine:
```
Build --> Export 
```

4.) Rename your exported html file to story.html

5.) Move story.html into the project directory /tmp

6.) Decompile the project with:
```sh
tweego -d -o tmp/all.twee story.html (Wichtig in tmp)
```

7.) Copy changes from all.twee into the single twee files in /src. If necessary, create new files or adapt existing ones. 

8.) Test that the project compiles without errors:
```sh
tweego.exe src/ -o tmp/story.html
```

9.) After successful testing compile project to /out:
```sh
tweego.exe src/ -o out/story.html
```

9.) Commit all 

## Git for Noobies

### Some Introduction
Since the project becomes more and more complex, it is necessary to upgrade our way of developing o the next level. That means that this READMe will become your holy bible for expert developing, so read it, internalize it, live it.Otherwise your commits will not be merged to the protected master branch. You have been warned.

#### Commit Messages
Commit messages should make sense. This means that a commit message gives the developers information about what the commit contains.
A commit message like this "fixes" does not give any information about its commit. There is no reference to the content of the commit. This is important to make bugfixing easier. Another note for commit messages is that they generally start with a capital letter.

- Don't: "Fixed"
- Do: "CTF 4: Fixed responsive design for background"

So here is the syntax for any future commit messages:
```
Affiliation: What has been done
```

To eliminate any further confusion, here are some more examples:
- "CTF 8: Add the necessary file for downloading"
- "Mainpage: Add external css file"
- "Repository: Add title.png"

#### Branching
Normally when working with version control software, nobody works on the master branch. Therefor you need to create an own branch that contains a copy of the master branch. When work is finished, then create a merge request to the main branch. If you are able to merge, you can do it, otherwise put an @ to someone who is able to merge in the merge message.

### Git Commands
To avoid confusion about the git commands, here is a list of the most common git commands.

#### Add files
First, before starting to work pull the current state of the repository with:
```sh
git pull
```

Pulling makes it possible to obtain a local copy of the repository, which you can then work with.
After work has been done, you need to prepare a commit for pushing your work into the repository. 
Therefore you need the following commands:
```sh
git add
git commit -m "<Commit message>"
git push
```

#### Checkout a Branch
The git console shows the current branch. For switching branches you only need:
```sh
git checkout <Branch name to checkout>
```

#### Create a Branch
Firstly:
```sh
git pull
```

Then create a new branch from an existing one:
```sh
git checkout -b <Branch name> <Branch name to copy from>
```

Git will automatically switch to the new branch so you can start working on it.

Then you need to commit the new branch: 
```sh
git add
git commit -m "<Commit message>"
git push
```
# Image Sources
Background Images by Lara Laskowsky -> /out/img/4all/*.svg, /out/src/*
PC Background: https://www.pexels.com/de-de/foto/grauer-lenovo-flachbildschirm-zeigt-an-was-sie-lieben-neon-signage-1772120/

CTF1:
https://www.hippopx.com/en/assorted-books-shelf-school-library-study-knowledge-51883

CTF2:
https://pixabay.com/de/illustrations/frau-malen-aquarell-papier-kunst-4178302/

CTF4:
/out/img/ctf4/www.png by Marc Schmidt

CTF5:
https://www.pexels.com/de-de/foto/verschiedene-gemalde-383568/

CTF6:
https://pixabay.com/de/photos/wolf-winter-schnee-raubtier-frost-2043464/
https://pixabay.com/de/photos/jay-vogel-zweig-sitzend-schneefall-548381/
https://pixabay.com/de/photos/w%c3%b6lfe-wald-winterlich-einsamkeit-1341881/

CTF7:
https://i0.hippopx.com/photos/440/457/108/books-shelf-school-library-preview.jpg

CTF8:
https://www.pexels.com/de-de/foto/foto-eines-verlassenen-arbeitsbereichs-3359003/

# Credits
