# Twine CTF

![](/lara/Title.png)

## Git for Noobies

### Some Introduction
Since the project becomes more and more complex, it is necessary to upgrade our way of developing o the next level. That means that this READMe will become your holy bible for expert developing, so read it, internalize it, live it.Otherwise your commits will not be merged to the protected master branch. You have been warned.

#### Branching
Normally when working with version control software, nobody works on the master branch. Therefor you need to create an own branch that contains a copy of the master branch.

Create a new branch from an existing one:
```sh
git checkout -b <Branch name> <Branch name to copy from>
```

Then you need to commit the new branch: 

### Git Commands
The very first thing to always do:
```sh
git pull
```

#### Add files
First, pull the current state of the repository with:
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

## CTF-Challenges Ideas

### Web
- XSS
- Injection
- CSRF Vulnerabilities

### Cryptography

### Binary Exploitation
- Buffer Overflow


### Workflow 

- Workflow: 

- 1.) git pull
- 2.) build your local twine project to work on in -> tweego.exe src/ -o out/story.html / (in src sollen immer die aktuellen files liegen)
- 3.) import story.html in your twine (work on it) if finished export twine --> Build --> export (als datei veröffentlichen)
- 4.) Decompile  project with tweego -d -o tmp/all.twee example5.html (Wichtig in tmp)
- 5.) Copy changes from all.twee in src/ (if necessary create new files and update main files)
- 6.) Test if story compiles with out errors if not correct errors tweego.exe src/ -o tmp/story.html
- 7.) Commit all (/tmp ist egal)
