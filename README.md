# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Lejia Zhao**

Time spent: **5** hours spent in total

Link to project: (https://rectangular-gem-seaplane.glitch.me)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:



## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
N/A

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
A challenge I encountered in the process was that after pressing the start button to start the game, the first clue would play and the corresponding button would light-up but it would stay lit-up. If the user presses the correct corresponding button, nothing happens, the button just stays lit-up from the first play of the clue. I have to restart the run time for the game to reset. I first thought that there was something wrong with my existing code - maybe I forgot to call the clearButton function in my play clue function or something of that sort. I looked over my code again and again but everything made sense to me. Then, I pulled up the console in my browser and discovered that there seemed to be a lot of errors related to the portion of the code involving AudioContext. Specifically, there was an error message that said “Can’t find variable AudioContext”. I was a bit confused because I had followed all the instructions. I decided to read the supplementary background information again more thoroughly. In the “Creating Sounds with AudioContext'' tutorial linked in the prework document, I found that the example given in the tutorial where they implemented AudioContext included an additional line of code before they initialized the AudioContext object. I tried writing the same line of code before my initialization of AudioContext, and miraculously the error in my code was  fixed. The clues could now play normally and the game is able to run smoothly. This process of debugging definitely took up a big chunk of my time when trying to implement this game, but when I finally figured it out, it was very rewarding. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
After completing my submission, I curious to learn more about how to implement more interactice features in the browser using javascript.

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had more time to work on this project, I would definitely implement all the optional features listed in the project description. Additionally, I would like to include a feature where(in that iteration of the run time) if the player gets every round right, the number of  button presses the user has to complete would increase. I would also like to add a feature that would keep track of the historical high scores of the user. 





## License

    Copyright [Lejia Zhao]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
