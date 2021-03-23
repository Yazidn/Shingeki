# Shingeki
A shell script to read Attack On Titan manga locally.

### Description
You have the option to use it with dmenu or fzf, or without both and you manually pass the chapter number as an only argument and it will act the same way the other two do, except for the prompt. You can also use `fromto` to download a range of chapters all at once.

### Requirements
+ curl
+ pup
+ dmenu (optional)
+ fzf (optional)

### Usage
#### dmenu & fzf
Make sure it is set to executable before you try to run it (it probably is, already.), when it runs, you'll see either a dmenu prompt or fzf depending on what you chose to go with, where you can search and select the chapter you want, once you make your selection, the corresponding pages will be downloaded to your home folder under a "manga" folder, unless specified otherwise in **DWNDIR** in the script.

#### manual
Run the script and supply the number of the chapter to be downloaded as follows: `./shingeki 9.1` (Yes, this is chapter 9.1 in this case, you can use 'print_possible_chapter_numbers' to know which numbers you can supply.

#### fromto
This makes it easier to download a range of chapters all at once, you use it by launching from the terminal and supplying the start and end chapter as follows: `./fromto 8 18`, this will download the chapters from 8 and 18, including the chapters that are not numbered ordinarily.

### Extras
I personally use **feh** for viewing images, therefore I added an **alias** in my __.bashrc__ that uses feh with some other commands that make sure I can immediately start reading in fullscreen and have the pages sorted accordingly, if you use **feh**, then this should work for you as well. `alias mng='feh -S mtime --reverse -F'`
