# FindReplace

## Introduction
An Ubuntu ``.deb`` package/command line utility that mimics Find/Replace functionality available in most Text Editors.
If you don't want to open a Text Editor or remember ``sed`` syntax for replacing strings in a text file, use ``findreplace``. It asks you to enter the word you wan't to replace & also checks if the word is present or not. If word is present, it prompts you to enter a word that you to be replaced with.
Its a wrapper built around ``sed``, hence its highly portable.

## Installation
Grab the ``.deb`` package from the [Release](https://github.com/shashank-ssriva/FindReplace/releases) & install it as : -
```
root@shashank-dbserver:/home/shashank# dpkg -i findreplace_0.2-1_all.deb
```
## Usage
Just execute ``findreplace`` command & pass a valid file-name where you want text to be substituted.
```
root@shashank-dbserver:/home/shashank# findreplace test.txt

Welcome to findreplace! A cute, little utility that mimics Find/Replace functionality available in most Text Editors. No more struggling with syntax :-)

Safety first! Hence, backing up the original file as 'test.txt.findreplace.orig'...

Enter the word you want to replace...tomatoes

Searching for 'tomatoes' in test.txt...

Word 'tomatoes' encountered 1 time(s). Good to go ahead with replacement ;-)

Enter what you want 'tomatoes' to be replaced with...potatoes

Replacing 'tomatoes' with 'potatoes'...

Below is your edited file displaying only the line(s) containing replaced text.

I love potatoes.

Hope you liked it ;-)
```
