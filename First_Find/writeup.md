# First Find
## Description
Unzip this archive and find the file named 'uber-secret.txt'
[Download zip file](https://artifacts.picoctf.net/c/502/files.zip)
## Solution
On unzipping the file and looking at the file structure:
```
❯ ls -a
.  ..  13771.txt.utf-8  14789.txt.utf-8  acceptable_books  adequate_books  satisfactory_books
```
Seeing that there are multiple folders, we will use grep:
```
❯ grep -R "pico" *
14789.txt.utf-8:brassa un picotin d'orge_. Comme depuis une demi-heure environ c'était
adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt:picoCTF{f1nd_15_f457_ab443fd1}
```
The flag is: ``picoCTF{f1nd_15_f457_ab443fd1}``


