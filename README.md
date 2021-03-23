# Shingeki
A shell script to read Attack On Titan manga locally.

### Description
You have the option to use it with dmenu or fzf, or without both and you manually pass the chapter number as an only argument and it will act the same way the other two do, except for the prompt.

### Requirements
+ curl
+ pup
+ dmenu (optional)
+ fzf (optional)

### Usage
Make sure it is set to executable before you try to run it, when it runs, you'll see a dmenu prompt where you can search and select the chapter you want, once you make your selection, the corresponding pages will be downloaded to your home folder under a "manga" folder, unless specified otherwise in **DWNDIR** in the script.

### Extras
I personally use **feh** for viewing images, therefore I added an **alias** in my __.bashrc__ that uses feh with some other commands that make sure I can immediately start reading in fullscreen and have the pages sorted accordingly, if you use **feh**, then this should work for you as well. `alias mng='feh -S mtime --reverse -F'`
