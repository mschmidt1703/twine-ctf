# Memory Loss: Find Your Way Back

<img src="/out/src/img/header/logo.svg" alt="Logo" width="75%"/>

Please use the online version to play this game: 
<a href="https://mschmidt1703.github.io/twine-ctf/" target="_blank">Click here to play</a>

This game was developed on the Twine engine to teach some basic knowledge about IT security and vulnerabilities using CTFs.

# Table of contents
1. [Memory Loss: Find Your Way Back](#memory-loss-find-your-way-back)
    1. [Overview of CTFs](#overview-of-ctfs)
    2. [How to start the Game](#how-to-start-the-game)
2. [Development](#development)
    1. [Requirements](#requirements)
    2. [Tests](#tests)
    3. [Workflow](#workflow)
    4. [Dependencies](#Dependencies)
4. [Image Sources](#image-sources)
5. [Credits](#credits)

## Overview of CTF Categories
- XSS
- Cryptography
- Forensics
- Web Exploitation
- Reverse Engineering

## How to start the Game
Please use the online version to play this game: 
<a href="https://mschmidt1703.github.io/twine-ctf/" target="_blank">Click here to play</a>

Some error may occur, when playing on a html file.
1. Clone the repository
2. Change into /out
3. Double click to start the story.html

# Development
Everything you need to work with this project.

## Requirements
- Twine with Harlowe 3.3.1
- Tweego

## Tests
Tested on Windows with Chrome Version 108.0.5359.126 and Firefox 108.0.2 (64-Bit),
Tested on Ubuntu 18.04.2 with Firefox 108.0.2 (64-bit)
Resolution: 1920x1080

Missing: Responsive Design -> Resolution: 1920x1080

## Dependencies
All dependencies will be loaded from local source. But here is an overview of all used dependencies.

- <a href="https://fonts.cdnfonts.com/css/ocr-a-extended" target="_blank">Font</a> 
- <a href="https://www.npmjs.com/package/crypto-js" target="_blank">Crypto-JS</a>
- <a href="https://highlightjs.org/download/" target="_blank">highlight.min.js</a> 
- <a href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/agate.min.css" target="_blank">CSS for highlight.min.js</a>
- <a href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.7.0/styles/default.min.css" target="_blank">CSS for highlight.min.js</a>
- <a href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css" target="_blank">Bulma</a>

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
tweego -d -o tmp/all.twee tmp/story.html (In tmp!)
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
Background Images: \
/out/src/* by Lara Laskowsky \
/out/src/img/main/wires_landscape.svg by Lara Laskowsky \
/out/src/img/header/* by Lara Laskowsky 

Images Mainpage: \
/out/src/img/general/ctf/previews/preview_default.svg by Lara Laskowsky \
/out/src/img/main/* by Lara Laskowsky

Icons: \
https://www.flaticon.com/de/kostenloses-icon/fragezeichen_5726470?term=fragezeichen&related_id=5726470 \
https://freeicons.io/material-icons-action/home-icon-15944 \
https://www.iconfinder.com/icons/2124268/document_essential_app_code_icon \
https://www.iconfinder.com/icons/1891021/approved_check_checkbox_checkmark_confirm_success_yes_icon \
https://www.iconfinder.com/icons/2303177/bulb_creative_hint_idea_lamp_light_tip_icon 

Icon Adaptions: \
/out/src/img/general/ctf/* by Lara Laskowsky 

Computer: \
https://www.pexels.com/de-de/foto/grauer-lenovo-flachbildschirm-zeigt-an-was-sie-lieben-neon-signage-1772120/ 

Adaption Background with computer: \
/out/src/img/general/ctf/pc_rahmen.png by Marc Schmidt 

CTF1: \
https://www.hippopx.com/en/assorted-books-shelf-school-library-study-knowledge-51883 

CTF2: \
https://pixabay.com/de/illustrations/frau-malen-aquarell-papier-kunst-4178302/ 

CTF4: \
/out/img/ctf4/www.png by Marc Schmidt 

CTF5: \
https://www.pexels.com/de-de/foto/verschiedene-gemalde-383568/ 

CTF6: \
https://pixabay.com/de/photos/wolf-winter-schnee-raubtier-frost-2043464/ \
https://pixabay.com/de/photos/jay-vogel-zweig-sitzend-schneefall-548381/ \
https://pixabay.com/de/photos/w%c3%b6lfe-wald-winterlich-einsamkeit-1341881/ 

CTF7: \
https://i0.hippopx.com/photos/440/457/108/books-shelf-school-library-preview.jpg 
