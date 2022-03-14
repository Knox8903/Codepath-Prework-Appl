# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Samuel Knox

Time spent: 4 hours spent in total

Link to project: https://glitch.com/edit/#!/chambray-four-helmet

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [X] Game button appearance change goes beyond color (e.g. add an image)
* [X] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [X] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [X] Visible mistake counter
- [X] Extra graphical additions

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![X] http://g.recordit.co/yW2MaCwMix.gif Gameplay Loop
![X]http://g.recordit.co/JCi5iI82QT.gif Mistakes
![X]http://g.recordit.co/QBTnmwAlCK.gif Timeout
![X] http://g.recordit.co/Xvh2jLJIOO.gif Game Completion (you can't see the buttons move that well since, by this point in the game, the clues are pretty fast)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
Stackoverflow (https://stackoverflow.com/questions/6910049/on-a-css-hover-event-can-i-change-another-divs-styling)

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
Three challenges arose while implementing some optional features. Specifically, the image buttons, audio buttons, and timer caused some problems. 

While implementing the image buttons, I had trouble affecting the CSS rules of one image when another is pressed. 
In fact, I spent the most time of trying to fix that problem. I ended up being able to find a Stackoverflow post about changing one element's style when hovering over another, and just modified the answer to fit my needs. 

The second issue was implementing sounds when a button was pressed. Aside from the obvious labor done by replacing a lot of code to accept sound and also removing code that was no longer necessary, it was pretty easy. 
The hard part, however, arose when I realized that the audio would be stopped short by the code that was previously meant to stop the tone that played. 
The problem was that it sounded extremely buggy when the audio was stopped short, so I decided to remove the code that stopped the audio when the button was lifted. 
Then, I found that overlapping audio wasn't allowed initially, so I looked around for a way to allow the audio to overlap and got a pretty good answer which solved my problem. 

The final issue was failing to stop every timer that started, I know now that for every "setinterval", there should be a "clearinterval". 
I wish I knew that sooner, it would've saved me 30 minutes of pain.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
I found that making adjustments to my code to make it perform better, as well as being more efficient and modular felt pretty good when it worked out, so that's certainly a goal I have in mind. 
Another goal would be to make the webpage look more appealing and implement moving elements that could appeal to the user. 
Finally, I want to begin work in a group environment to see how well I would perform, I think I would do well since I like to hyper focus on one thing, so a situation where work is split up amongst individuals sounds very enjoyable. 
So for my questions, I would ask: how do I make my code more efficient, how do I make my CSS more appealing, and how enjoyable is group work in an organized environment?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had more time to work on this project, I would spend a lot of time cleaning up my code and making the interface more intuitive and look better. 
Specifically, I wanted to make a timer that would only show when the user has 3 seconds left, I also thought it would be cool if the timer would slide in from the left or right when this 3 second condition was active. 
I couldn't find time to implement this, though, since I wasn't sure how I could implement moving elements in an efficient way, I was also already having trouble making the timer work, so I ended up scrapping the idea since I still had things to complete. 
As for cleaning up my code, some of my solutions to problems don't feel very stable, and instead feel like they were just patched together until it was working. 
I also wanted to show a progress bar to show how many patterns were left, and to compliment this, I also wanted to make a difficulty system that would increase the number of patterns. 
In fact, I even made the speed increase feature (the one listed in optional features) scalable, in order to allow for a higher number of patterns. 
Its a shame I couldn't implement these features, but I have to submit it at some point, right?



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright Samuel Knox

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.