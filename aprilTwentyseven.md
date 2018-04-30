## April 27th, 2018
#### Overview and Learning
Throughout this week, the goal was to continue learning but to also start the building of the tutorial. This is when my independent project enters its next stage. The first step was to read through sources and start to learn about the topic and to try and get to a place where I am comfortable with the topic. The next step is to start gathering information and to start creating examples because a tutorial is only as good as the explanation that is provided. With the actual formation of the tutorial on the back of my mind, I decided to further my knowledge on the topic and continue digging into `sed`. I found some `sed` commands that are not regularly used and I decided to dive in depth. <br>

`sed 'y/abcdefghij/0123456789'`<br>
The line above reads like this. The a-j provides a span of letters and the numbers provide the range that the programmer wishes to edit. This line of code is rarely used because changing certain ranges of letters to numbers isn't efficient, but perhaps it may be used to encode messages. Anyway, lets say your textfile looks like this: <br>
```
Horse, cow, car, hello
``` 
<br>
And then you apply `sed 'y/abcdefghij/0123456789'` to it, your file should then switch to:
```
7ors4, 2ow, 20r, 74llo
``` 
<br>
At this point I will start typing in lines of code, since this is a journal, and I will start providing explanations since I need to get ready to make the tutorial. <br>

1. `sed '3a alvin'` <br>
This tells the computer to append the line that follows 'line 3' and the word that follows `3a` is the word that will be added, although the space will not be included. 
2. `sed '2i hello'` <br>
this line is basically the inverse of the first one and all it does insert the word before the line that is specified. 

#### Takeaways 
Throughout the course of this project, there is only one thing that has really stuck out to me. It's not what you learn, or the knowledge that you accumulate, rather it is that this is only temporary and that you need gain the benefits of what it is your as soon as possible because everything moves forward whether and you need to move with it without dwelling on what you could've done or not done. I say this because as we move forward with the project, there is no point of looking back wishing that we could have worked on something for longer . instead we need to take the knowledge that we have already atttained and continue moving forward, and I feel like college will be similar. 
<br>
[Next](mayFour.md)<br>
[Previous](aprilTwenty.md)<br>
[Table of Contents](readme.md)