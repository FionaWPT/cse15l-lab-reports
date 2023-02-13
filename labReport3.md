# Four command-line options for `grep`
# 1. `-c`
The `-c` command-line option prints the number count of the lines of specified words within a certain file.
We use `-c` like this: `grep -c "words you want to find" path of the file or name of the file`.
## Two examples of `-c`
```js
//Example 1:
$ grep -c "The Nara Period" ./written_2/travel_guides/berlitz1/HistoryJapan.txt
1
//This code shows the number count of lines that contain the word 
//"The Nara Period" in the file named HistoryJapan. 
//This is useful when you want to know if this text contains the topic 
//you are looking for before you start reading a long text. 
//If you know the file does not have the topic you are searching for, 
//then that saves your time looking through the text.
```
```js
//Example 2:
$ grep -c "Japan" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HandRHawaii.txt:0
./written_2/travel_guides/berlitz1/HandRHongKong.txt:0
./written_2/travel_guides/berlitz1/HandRIbiza.txt:0
./written_2/travel_guides/berlitz1/HandRIsrael.txt:0
./written_2/travel_guides/berlitz1/HandRIstanbul.txt:0
./written_2/travel_guides/berlitz1/HandRJamaica.txt:1
./written_2/travel_guides/berlitz1/HandRJerusalem.txt:0
./written_2/travel_guides/berlitz1/HandRLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/HandRLasVegas.txt:0
./written_2/travel_guides/berlitz1/HandRLisbon.txt:0
./written_2/travel_guides/berlitz1/HandRLosAngeles.txt:0
./written_2/travel_guides/berlitz1/HandRMadeira.txt:0
./written_2/travel_guides/berlitz1/HandRMadrid.txt:0
./written_2/travel_guides/berlitz1/HandRMallorca.txt:0
./written_2/travel_guides/berlitz1/HistoryDublin.txt:0
./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:0
./written_2/travel_guides/berlitz1/HistoryEgypt.txt:0
./written_2/travel_guides/berlitz1/HistoryFrance.txt:0
./written_2/travel_guides/berlitz1/HistoryFWI.txt:0
./written_2/travel_guides/berlitz1/HistoryGreek.txt:0
./written_2/travel_guides/berlitz1/HistoryHawaii.txt:6
./written_2/travel_guides/berlitz1/HistoryHongKong.txt:6
./written_2/travel_guides/berlitz1/HistoryIbiza.txt:0
./written_2/travel_guides/berlitz1/HistoryIndia.txt:3
./written_2/travel_guides/berlitz1/HistoryIsrael.txt:0
./written_2/travel_guides/berlitz1/HistoryIstanbul.txt:0
./written_2/travel_guides/berlitz1/HistoryItaly.txt:0
./written_2/travel_guides/berlitz1/HistoryJamaica.txt:0
./written_2/travel_guides/berlitz1/HistoryJapan.txt:101
./written_2/travel_guides/berlitz1/HistoryJerusalem.txt:0
./written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/HistoryLasVegas.txt:0
./written_2/travel_guides/berlitz1/HistoryMadeira.txt:0
./written_2/travel_guides/berlitz1/HistoryMadrid.txt:0
./written_2/travel_guides/berlitz1/HistoryMalaysia.txt:21
./written_2/travel_guides/berlitz1/HistoryMallorca.txt:0
./written_2/travel_guides/berlitz1/IntroDublin.txt:0
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:0
./written_2/travel_guides/berlitz1/IntroEgypt.txt:0
./written_2/travel_guides/berlitz1/IntroFrance.txt:0
./written_2/travel_guides/berlitz1/IntroFWI.txt:0
./written_2/travel_guides/berlitz1/IntroGreek.txt:0
./written_2/travel_guides/berlitz1/IntroHongKong.txt:0
./written_2/travel_guides/berlitz1/IntroIbiza.txt:0
./written_2/travel_guides/berlitz1/IntroIndia.txt:1
./written_2/travel_guides/berlitz1/IntroIsrael.txt:0
./written_2/travel_guides/berlitz1/IntroIstanbul.txt:0
./written_2/travel_guides/berlitz1/IntroItaly.txt:0
./written_2/travel_guides/berlitz1/IntroJamaica.txt:0
./written_2/travel_guides/berlitz1/IntroJapan.txt:50
./written_2/travel_guides/berlitz1/IntroJerusalem.txt:0
./written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/IntroLasVegas.txt:0
./written_2/travel_guides/berlitz1/IntroLosAngeles.txt:1
./written_2/travel_guides/berlitz1/IntroMadeira.txt:0
./written_2/travel_guides/berlitz1/IntroMadrid.txt:0
./written_2/travel_guides/berlitz1/IntroMalaysia.txt:0
./written_2/travel_guides/berlitz1/IntroMallorca.txt:0
./written_2/travel_guides/berlitz1/JungleMalaysia.txt:0
./written_2/travel_guides/berlitz1/WhatToDublin.txt:0
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:0
./written_2/travel_guides/berlitz1/WhatToEgypt.txt:1
./written_2/travel_guides/berlitz1/WhatToFrance.txt:0
./written_2/travel_guides/berlitz1/WhatToFWI.txt:1
./written_2/travel_guides/berlitz1/WhatToGreek.txt:0
./written_2/travel_guides/berlitz1/WhatToHawaii.txt:0
./written_2/travel_guides/berlitz1/WhatToHongKong.txt:3
./written_2/travel_guides/berlitz1/WhatToIbiza.txt:0
./written_2/travel_guides/berlitz1/WhatToIndia.txt:0
./written_2/travel_guides/berlitz1/WhatToIsrael.txt:0
./written_2/travel_guides/berlitz1/WhatToIstanbul.txt:0
./written_2/travel_guides/berlitz1/WhatToItaly.txt:0
./written_2/travel_guides/berlitz1/WhatToJamaica.txt:0
./written_2/travel_guides/berlitz1/WhatToJapan.txt:63
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt:0
./written_2/travel_guides/berlitz1/WhatToLosAngeles.txt:1
./written_2/travel_guides/berlitz1/WhatToMadeira.txt:0
./written_2/travel_guides/berlitz1/WhatToMalaysia.txt:0
./written_2/travel_guides/berlitz1/WhatToMallorca.txt:0
./written_2/travel_guides/berlitz1/WhereToDublin.txt:3
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt:0
./written_2/travel_guides/berlitz1/WhereToEgypt.txt:0
./written_2/travel_guides/berlitz1/WhereToFrance.txt:2
./written_2/travel_guides/berlitz1/WhereToFWI.txt:0
./written_2/travel_guides/berlitz1/WhereToGreek.txt:0
./written_2/travel_guides/berlitz1/WhereToHawaii.txt:0
./written_2/travel_guides/berlitz1/WhereToHongKong.txt:6
./written_2/travel_guides/berlitz1/WhereToIbiza.txt:0
./written_2/travel_guides/berlitz1/WhereToIndia.txt:3
./written_2/travel_guides/berlitz1/WhereToIsrael.txt:0
./written_2/travel_guides/berlitz1/WhereToIstanbul.txt:0
./written_2/travel_guides/berlitz1/WhereToItaly.txt:0
./written_2/travel_guides/berlitz1/WhereToJapan.txt:214
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt:0
./written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:0
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:6
./written_2/travel_guides/berlitz1/WhereToMadeira.txt:0
./written_2/travel_guides/berlitz1/WhereToMadrid.txt:1
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt:20
./written_2/travel_guides/berlitz1/WhereToMallorca.txt:0
//This code shows the number count of lines in each files in the 
//directory berlitz1 that contains the word "Japan".
//This is useful when you want to know which files do not talk about Japan 
//and which files do talk about Japan. 
//From the files that talk about Japan, you can also know 
//which specific file spends more texts to talk about Japan.
```
# 2. `-l`
The `-l` command-line option prints the path of the files that contains a specified words.
We use `-l` like this: `grep -l "words" path`.
## Two examples of `-l`
```js
//Example 1:
$ grep -l "Japan" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HandRJamaica.txt
./written_2/travel_guides/berlitz1/HistoryHawaii.txt
./written_2/travel_guides/berlitz1/HistoryHongKong.txt
./written_2/travel_guides/berlitz1/HistoryIndia.txt
./written_2/travel_guides/berlitz1/HistoryJapan.txt
./written_2/travel_guides/berlitz1/HistoryMalaysia.txt
./written_2/travel_guides/berlitz1/IntroIndia.txt
./written_2/travel_guides/berlitz1/IntroJapan.txt
./written_2/travel_guides/berlitz1/IntroLosAngeles.txt
./written_2/travel_guides/berlitz1/WhatToEgypt.txt
./written_2/travel_guides/berlitz1/WhatToFWI.txt
./written_2/travel_guides/berlitz1/WhatToHongKong.txt
./written_2/travel_guides/berlitz1/WhatToJapan.txt
./written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
./written_2/travel_guides/berlitz1/WhereToDublin.txt
./written_2/travel_guides/berlitz1/WhereToFrance.txt
./written_2/travel_guides/berlitz1/WhereToHongKong.txt
./written_2/travel_guides/berlitz1/WhereToIndia.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
./written_2/travel_guides/berlitz1/WhereToMadrid.txt
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt
//This code prints only the files that contains the word 
//"Japan" in the directory of berlitz1
//instead of printing out all the files that 
//include files that does not have "Japan".
//This is useful when you only wnat to check what files contain 
//a certain words no matter the number count of it. 
//You can also use `-c` to reach the same goal but 
//it would be hard to read if you only want to see files that 
//contain the words since it shows all the files in the terminal.
```
```js
//Example 2:
$ grep -l "Theory of Relativity" ./written_2/travel_guides/berlitz2/*.txt
./written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt
//This code prints the only file that contains "Theory of Relativity" in the directory berlitz2.
//This is useful to save your time find the words one by one in each text files. 
//You can quickly locate the file in this way.
```
# 3. `-n`
The `-n` command-line option prints the lines that contains the specified words with the line number before.
We use `-n` like this: `grep -n "words" path`.
## Two examples of `-n`
```js
//Example 1:
$ grep -n "Hawaiians" ./written_2/travel_guides/berlitz1/HistoryHawaii.txt
28:        might seem less than Edenic, the early Hawaiians led a pleasurable
127:        Hawaiians were opposed to surrendering their sovereignty. When a new
141:        Hawaiians were finding themselves overwhelmed and outnumbered. Disease
169:        Political and economic power resided with non-Hawaiians. Dole and other
176:        Japanese in Hawaii outnumbered Hawaiians two to one.
223:        component was a growing movement by native Hawaiians to restore the
// This code prints out the line numbers and the sentences 
//that contains the specific word “Hawaiians" 
// in the file named HistoryHwaii.
// This is useful when you want to know the exact lines 
//that contain certain words and thier locations in the text file. 
```
```js
//Example 2:
$ grep -n "Aloha" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HistoryHawaii.txt:166:        famous, Aloha Oe.
./written_2/travel_guides/berlitz1/HistoryHawaii.txt:182:        Line soon were arriving regularly at Aloha Tower, bearing tourists 
from
./written_2/travel_guides/berlitz1/WhatToHawaii.txt:37:        landing) who nest there. Aloha Airlines offers scheduled flights to
// This code prints out not only the line numbers and the sentences 
// that contains the word "Aloha"
// but it also prints out the path of the files since we let the computer 
// to find in all the text files in berlitz1.
// This is useful when you want to know which text files 
// in a certain directory contains certain words 
// and the locations of the words.
```
# 4. `-L`
This `-L` command-line option prints out the file names that do not contain a specified words.
We use `-L` like this: `grep -L "words" path`.
## Two examples of `-L`
```js
//Example 1:
$ grep -L "History" ./written_2/travel_guides/berlitz1/*.txt
./written_2/travel_guides/berlitz1/HandRHawaii.txt
./written_2/travel_guides/berlitz1/HandRHongKong.txt
./written_2/travel_guides/berlitz1/HandRIbiza.txt
./written_2/travel_guides/berlitz1/HandRIsrael.txt
./written_2/travel_guides/berlitz1/HandRIstanbul.txt
./written_2/travel_guides/berlitz1/HandRJamaica.txt
./written_2/travel_guides/berlitz1/HandRJerusalem.txt
./written_2/travel_guides/berlitz1/HandRLakeDistrict.txt
./written_2/travel_guides/berlitz1/HandRLasVegas.txt
./written_2/travel_guides/berlitz1/HandRLisbon.txt
./written_2/travel_guides/berlitz1/HandRLosAngeles.txt
./written_2/travel_guides/berlitz1/HandRMadeira.txt
./written_2/travel_guides/berlitz1/HandRMadrid.txt
./written_2/travel_guides/berlitz1/HandRMallorca.txt
./written_2/travel_guides/berlitz1/HistoryFrance.txt
./written_2/travel_guides/berlitz1/HistoryIndia.txt
./written_2/travel_guides/berlitz1/HistoryItaly.txt
./written_2/travel_guides/berlitz1/HistoryMadrid.txt
./written_2/travel_guides/berlitz1/IntroDublin.txt
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt
./written_2/travel_guides/berlitz1/IntroEgypt.txt
./written_2/travel_guides/berlitz1/IntroFrance.txt
./written_2/travel_guides/berlitz1/IntroFWI.txt
./written_2/travel_guides/berlitz1/IntroGreek.txt
./written_2/travel_guides/berlitz1/IntroHongKong.txt
./written_2/travel_guides/berlitz1/IntroIbiza.txt
./written_2/travel_guides/berlitz1/IntroIndia.txt
./written_2/travel_guides/berlitz1/IntroIsrael.txt
./written_2/travel_guides/berlitz1/IntroIstanbul.txt
./written_2/travel_guides/berlitz1/IntroItaly.txt
./written_2/travel_guides/berlitz1/IntroJamaica.txt
./written_2/travel_guides/berlitz1/IntroJapan.txt
./written_2/travel_guides/berlitz1/IntroJerusalem.txt
./written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
./written_2/travel_guides/berlitz1/IntroLasVegas.txt
./written_2/travel_guides/berlitz1/IntroLosAngeles.txt
./written_2/travel_guides/berlitz1/IntroMadeira.txt
./written_2/travel_guides/berlitz1/IntroMadrid.txt
./written_2/travel_guides/berlitz1/IntroMallorca.txt
./written_2/travel_guides/berlitz1/JungleMalaysia.txt
./written_2/travel_guides/berlitz1/WhatToDublin.txt
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt
./written_2/travel_guides/berlitz1/WhatToEgypt.txt
./written_2/travel_guides/berlitz1/WhatToFrance.txt
./written_2/travel_guides/berlitz1/WhatToFWI.txt
./written_2/travel_guides/berlitz1/WhatToGreek.txt
./written_2/travel_guides/berlitz1/WhatToHawaii.txt
./written_2/travel_guides/berlitz1/WhatToHongKong.txt
./written_2/travel_guides/berlitz1/WhatToIbiza.txt
./written_2/travel_guides/berlitz1/WhatToIndia.txt
./written_2/travel_guides/berlitz1/WhatToIsrael.txt
./written_2/travel_guides/berlitz1/WhatToIstanbul.txt
./written_2/travel_guides/berlitz1/WhatToItaly.txt
./written_2/travel_guides/berlitz1/WhatToJapan.txt
./written_2/travel_guides/berlitz1/WhatToLakeDistrict.txt
./written_2/travel_guides/berlitz1/WhatToLasVegas.txt
./written_2/travel_guides/berlitz1/WhatToMadeira.txt
./written_2/travel_guides/berlitz1/WhatToMalaysia.txt
./written_2/travel_guides/berlitz1/WhatToMallorca.txt
./written_2/travel_guides/berlitz1/WhereToEdinburgh.txt
./written_2/travel_guides/berlitz1/WhereToEgypt.txt
./written_2/travel_guides/berlitz1/WhereToFrance.txt
./written_2/travel_guides/berlitz1/WhereToGreek.txt
./written_2/travel_guides/berlitz1/WhereToHawaii.txt
./written_2/travel_guides/berlitz1/WhereToIbiza.txt
./written_2/travel_guides/berlitz1/WhereToIndia.txt
./written_2/travel_guides/berlitz1/WhereToIsrael.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToMadeira.txt
./written_2/travel_guides/berlitz1/WhereToMadrid.txt
./written_2/travel_guides/berlitz1/WhereToMallorca.txt
// This code prints out all the files in the directory berlitz1 
// that do not have the words "History".
// This is useful when you want to exclude files that contains certain words.
```
```js
//Example 2:
$ grep -L "." ./written_2/travel_guides/berlitz1/*.txt

// This code also prints out all the files in the directory berlitz1 
// that do not have the words ".".
// Aparently, nothing is printed out because all the files contain a period ".".
//This is useful when you want to check if certain words exists in all the files.
```
# Resources
I used ChatGPT to provide me examples and descriptions of command-line options for `grep` and I chose four of them. 
I typed all the code myself in VS code.
