## Friday, April 13th, 2018
#### Overview and Learning
This week I started getting into `sed` and `awk`. And so far I can say that I prefer it over `grep`. `sed` and `awk` are very similar to each other but they are completely different from `grep`. `sed` and `awk` can be classified as "text processors" while `grep` is more of a search engine, that searches for certain terms inside of individual files. These classifications can go further, as `sed` and `awk` do have their differences. `sed` focuses more on the editing of certain files and it allows you to adjust and alter files without leaving the command line. Throughout this week, I began to get into `sed` and I have to admit that I do like it better than `grep`. An example of `sed` would be this:
```
sed 's/hello/world/' input.txt > output.txt
```
The line of code above basically tells the computer to switch every "hello" to a "world" throughout the entire document. This little simple example goes to show you how powerful `sed` and the command line could be, because it allows the programmer to switch and edit files without having the programmer open every single document. Another capability of `sed` is that it is able to print certain lines in particular documents. The line of code to do this would be:
```
sed -n '45p' file.txt
```
In the code snippet above the number obviously refers to the line in the document and the 'p' gives the order to print, followed by the name of the file. 

**Was not able to complete a full week of research because of a college trip that lasted three days**



[Previous](/marchThirty.md)<br>
[Next](/aprilTwenty.md)<br>
[Table of Contents](/readme.md)