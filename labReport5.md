# Four command-line options for `find`
# 1. `-name`
The `-name` command-line option shows the path of a specific file.
We use `-name` like this: `find -name "file name"`.
## Two examples of `-name`
__Example 1:__
```js
$ find -name HistoryFrance.txt
./written_2/travel_guides/berlitz1/HistoryFrance.txt

//This code shows the path of the file named HistoryFrance.
//This is useful when you want to find a certain file
//but you forgot where the file is saved.
```
__Example 2:__
```js
$ find -name berlitz1
./written_2/travel_guides/berlitz1

//This code shows where the folder berlitz1 is stored.
//This is useful when you want to find the folder but
//you forgot where the folder is.
```
# 2. `-type`
The `-type` command-line option shows all the files of a certain type in
the current directory.
We use `-type` like this: `find -type f/d/l`. (depends on what type you
are searching for)
## Two examples of `-l`
__Example 1:__
```js
$ find -type d
.
./.git
./.git/hooks
./.git/info
./.git/logs
./.git/logs/refs
./.git/logs/refs/heads
./.git/logs/refs/remotes
./.git/logs/refs/remotes/origin
./.git/logs/refs/remotes/upstream
./.git/objects
./.git/objects/info
./.git/objects/pack
./.git/refs
./.git/refs/heads
./.git/refs/remotes
./.git/refs/remotes/origin
./.git/refs/remotes/upstream
./.git/refs/tags
./lib
./written_2
./written_2/non-fiction
./written_2/non-fiction/OUP
./written_2/non-fiction/OUP/Abernathy
./written_2/non-fiction/OUP/Berk
./written_2/non-fiction/OUP/Castro
./written_2/non-fiction/OUP/Fletcher
./written_2/non-fiction/OUP/Kauffman
./written_2/non-fiction/OUP/Rybczynski
./written_2/travel_guides
./written_2/travel_guides/berlitz1
./written_2/travel_guides/berlitz2

//This code shows all the directories in the current directory doresearch
//This is useful when you want to search for all the directories. 
```
__Example 2:__
```js
$ find -type l


//This code shows all the symbolic link in the current directory.
//This shows that there is no symbolic link in the directory doresearch.
//This is useful when you want to find all symbolic links in the directory.
```
# 3. `-size`
The `-size` command-line option shows the path of the files that have a
specified size in terms of bytes.
We use `-s ize` like this: `find -size n`. (where n is the number of bytes)
## Two examples of `-size`
__Example 1:__
```js
$ find -size 4
./.git/hooks/pre-commit.sample
./Server.java
./written_2/travel_guides/berlitz1/HandRLakeDistrict.txt
./written_2/travel_guides/berlitz1/HandRLasVegas.txt

//This code shows all the path of files that have 4 bytes. 
//This is useful when you want to know how many a certain size 
//of the files are there. It is also useful when you only want
//to find shorter articles or longer articles to read.
```
__Example 2:__
```js
$ find -size 16
./written_2/travel_guides/berlitz1/IntroDublin.txt
./written_2/travel_guides/berlitz1/IntroEgypt.txt
./written_2/travel_guides/berlitz1/IntroFWI.txt
./written_2/travel_guides/berlitz2/Algarve-Intro.txt

// This code shows all the path of files that have 16 bytes.
// This is useful when you want to search for files that
// have a certain size. It is also useful when you want 
// to find relatively longer articles to read.
```
# 4. `-mmin`
This `-mmin` command-line option shows the files that are modified a certain
minitues ago.
We use `-mmin` like this: `find -mmin n`. (where n is the number of minutes)
## Two examples of `-mmin`
__Example 1:__
```js
$ find -mmin 1
./written_2/travel_guides/berlitz1/HandRLasVegas.txt

// This code shows the file that I modified one minute ago.
// This is useful when you want to quickly find the file you just edited
// when there are a lot of files and you forgot which one you edited.
```
__Example 2:__
```js
$ find -mmin 4
./written_2/travel_guides/berlitz1/HandRLasVegas.txt

// This code shows the same file I edited but it is now 4 minutes
// Again, this is useful when you want to find the file you modified quickly
// instead of scrolling through a bunch of files in the directory.
```
# Resources
I used ChatGPT to provide me examples and descriptions of command-line options for `find` and I chose four of them. 
I typed all the code myself in VS code.
