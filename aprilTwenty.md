## Friday, April 20th, 2018
#### Overview and Learning
Last week I did not get to get in depth as I wished. I was in Indiana visiting the college that I committed too. That being said my research and learning was cut short last week to only about two and a half days. Last week, I stated that `sed` and `awk` where more similar to eachother than `grep` was to either of them, and I decided to use that knowledge to focus my energy and attention on both `sed` and `awk` rather than `grep`. This week I want to start looking at other resources rather than just looking at one website and looking at their documentation, I want to branch out and see what videos and podcast are out there because I feel like learning will be easier if it is visual and auditory. I feel like Youtube will be a good resource to use because it is less formal and many different learning styles can be found, sometimes professionalism can be confusing, and a more relaxed explanation can actually allow you to process the information that you have learnt. While a video would be more helpful I decided to test my luck with another website. On that particular website I found the explanations to be less complicated because it was interpreted by a different software engineer, or perhaps another student who was having trouble understanding the complexity of the topic. While watching youtube videos, I realized that if you are trying to change multiple things about a textfile, having a several commands separated by commas can lead to confusion and errors. The easiest way to add multiple commands is to create a file with all of the commands you wish to apply, and then call both files together. For example: <br>
Lets say you have a text file, and in that file it says: 
```
three little pigs
one two three
peanut butter jelly
```
if you would like to change the lowercase "t's" to capital "T's," and change the lowercase "e's" to capital "E's," and also change lowercase "u's" to capital "U's" you can do this:
```
sed 's/t/T/g;s/e/E/d;s/u/U/g' textfile 
```
but as your commands get longer and longer, and as you add five, six, or maybe even seven to your command line, it will start to get confusing. This is where organization and new text files come in. The easiest way and "cleanest" way to make the above code snippet to happen is to make a new file. Said file would look like this:
```
s/t/T/g
s/e/E/g
s/u/U/g
```
The snippet above would tell the program what to do, and the only step left is to tell the computer what file to edit. Which looks like this:
```
sed -f filewithcommands textfile
```
on the snippet above, the `-f` just tells the computer to look at a particular file, the file name after points to what file to read first(`filewithcommands`), and then apply what it has read to the last file (`textfile`). Whether you tell the computer all the commands in the command line or whether you use a new file, the new `textfile`, should look like this:<br>
 ```
 ThrEE liTTlE pigs
 onE Two ThrEE
 pEanUT bUTTEr jElly
 ```