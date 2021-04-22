---
title: Overview
description: Project Summary and intended users
menu: Overview
order: 0
---
## Creators

* Hana Dawson
  * [LinkedIn](https://www.linkedin.com/in/hanadawson/)
  * Hdawsoncoder@gmail.com
  
* Kaz Penn
  * [LinkedIn](https://www.linkedin.com/in/kasmir-penn-a11127206/)
  * Kazpenn2020@gmail.com
  

## Summary

A top down dungeon maze game. Users will have to navigate through a maze within the given time per difficulty of level. 
The user can only see up to one space ahead of them and will have to memorize the corridors in order to pass through successfully. 

## Intended users

* People who like challenging puzzles.

  >As someone who likes puzzle games I would love to have a challenging game that requires me to really think about what I am doing and plan ahead with each move. 
  
* People who are casual gamers.

  >As someone who likes to play games, but not on consoles, I would love to have a game that allows me to play when I want, without the pressure of being judged if I am not good enough at the game, and knowing I can go at my own pace.
  
## Current state of the app

* On the home page, a user is able to generate a new maze by clicking the new button on the top bar
navigation. When the user clicks new, a maze is generated based on the current level selected in the
  preferences' menu.
    * Users can choose a difficulty level from 1-10, default being 4. This increases the size of the maze, which increases
  the corridors available for a user to go through.
  
* The user can navigate through the maze by clicking a direction on the 'd-pad' which displays
below the view of the maze. The user has a circle that is shown, starting at the starting cell, shown
  by a square, and have to navigate through the maze to the end cell which is also shown by a square
  marker.

* The user is able to switch to leaderboard in the bottom level navigation and see the current list of 
attempts listed in descending order starting from the lowest time to the highest time completed.
  
## Aesthetics to improve

* Update starting/ending markers to be more visually pleasing. Would like to make it no longer just 
  a colored square, but perhaps a slightly animated circular object that almost looks like a portal.
  

* Update the circle that shows the users current cell to be something more pleasing. Perhaps allow 
users to select from different characters, such as a mouse, a person or other types of characters.
  

* Updating the maze to have different colors on the ground. The ground may be dark at the starting of the
maze and get lighter the closer you get towards the end of the maze. This could be a good visual cue 
  for players to know they are getting closer to the end of the maze, especially once we implement the
  maze paths to be hidden from the user, when they can only see one cell at a time as they navigate through
  the maze.
  
## Functional Stretch goals

* Adding the option to allow users to have the maze hidden from view while going through the maze.
This would create a different style of game where the user can only see one cell at a time as they navigate
  through the maze. They could see their trail behind them, however when proceeding forward
  they would only be able to guess which way to go by which arrows on the controller are highlighted.
  

* Adding a timer based on difficulty for each level of maze. The user would then have to pass through the
maze within the time given, or else the game would end, and they would have to restart.
  
## Original Intended Functionality

* Users will be set in a grid-like maze and have to move through the maze while only seeing one step ahead at a time with the options of which direction they can go.

* Users will choose the direction of which way their "character" can go by tapping on the "d-pad" to choose an available direction to go.

* There will be levels of difficulty 1-20 that a user can select. The difficulty rating effects the amount of corridors the player may have to go through to find the exit. With each level of difficulty, the player is also allowed more time to get through the level.

* Each time a new maze is rendered, the corridors with be randomly generated. Players can choose to play the same difficulty over and over again but each time they start a new level it will be different.

* If a player runs out of time, they have the option to restart the maze and when doing so, the same maze will re-generate, and the player will have to memorize the paths they chose before to try to get to the end before running out of time.

* Players will have access to a leaderboard that will show ranks of levels beaten and high scores of the fastest times beaten in each difficulty.

## Device/external services

* Google sign in
>Google sign in will be used to track the users accomplishments for leaderboards (Levels beaten, time taken, etc...). Google sign in will also allow users to access their same accounts and stats through multiple devices.

## Stretch goals/possible enhancements

* Add different skins so players can change the look of their character

* Add music

* Add improved graphics

* Add Facebook log in

### Additional Information

[Summary of project](pdf/summary.pdf)

[API Docs](api/apidocs/index.html)

[ERD](https://dungeon-run.github.io/erd)

[Wireframe](https://dungeon-run.github.io/wireframe)

[Data Definition Language](https://dungeon-run.github.io/ddl)

[GitHub Links](https://dungeon-run.github.io/github-links)

[Build Instructions](build-instructions.md)

[Technology Inventory](https://dungeon-run.github.io/technology-inventory)

[Javadoc](api/apidocs/index.html)

## Copyright & License information
Copyright 2021 Hana Dawson, Kaz Penn

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

> <http://www.apache.org/licenses/LICENSE-2.0>
Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Additional copyright & license notices can be read in ['NOTICE'](NOTICE), [`docs/notice.md`](docs/notice.md), and ['LICENSE'](LICENSE) . 