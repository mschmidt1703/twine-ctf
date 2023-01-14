# Memory Loss: Find Your Way Back
![](title.png)

You can play this game online in your browser [here](https://mschmidt1703.github.io/twine-ctf/)

This game was developed on the Twine engine to teach some basic knowledge about IT security and vulnerabilities using CTFs.

# Table of contents
1. [Memory Loss: Find Your Way Back](#memory-loss-find-your-way-back)
    1. [Overview of CTFs](#overview-of-ctfs)
    2. [How to start the Game](#how-to-start-the-game)
2. [Development](#development)
    1. [Requirements](#requirements)
    2. [Workflow](#workflow)
3. [Image Sources](#image-sources)
4. [Credits](#credits)

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

3.) Copy all directories and story.html from /out in your twine folder. 

4.) If work is done then export html file from Twine:
```
Build --> Export 
```

5.) Rename your exported html file to story.html

6.) Move story.html into the project directory /tmp

7.) Decompile the project with:
```sh
tweego -d -o tmp/all.twee tmp/story.html (Wichtig in tmp)
```

8.) Copy changes from all.twee into the single twee files in /src. If necessary, create new files or adapt existing ones. 

9.) Test that the project compiles without errors:
```sh
tweego.exe src/ -o tmp/story.html
```

10.) After successful testing compile project to /out:
```sh
tweego.exe src/ -o out/story.html
```

11.) Commit all 

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

Icons:
https://www.flaticon.com/de/kostenloses-icon/fragezeichen_5726470?term=fragezeichen&related_id=5726470
https://freeicons.io/material-icons-action/home-icon-15944
https://www.iconfinder.com/icons/2124268/document_essential_app_code_icon
https://www.iconfinder.com/icons/1891021/approved_check_checkbox_checkmark_confirm_success_yes_icon
https://www.iconfinder.com/icons/2303177/bulb_creative_hint_idea_lamp_light_tip_icon

# Credits
