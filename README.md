# Twine CTF

![](/lara/Title.png)

## Git-Commands

### Add files
```sh
git add
git commit -m "Test"
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

## Credits
ctf2: https://pixabay.com/de/illustrations/frau-malen-aquarell-papier-kunst-4178302/
ctf7: https://i0.hippopx.com/photos/440/457/108/books-shelf-school-library-preview.jpg
