---
title: Projects
excerpt: "Projects"
aside: false
---

### Rail Sweeper
###### Unity Game Engine, C#, Blender, Unity Version Control
<br>

<iframe width="610" height="365" src="https://www.youtube.com/embed/A0G27q6DOSw?si=hkNj_AppI3YnGUAb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br>

##### Repo
[GitHub - Rail Sweeper](https://github.com/Jsomerville1/RailSweeper)

#### Download
[Itch.io - Rail Sweeper](https://joeso.itch.io/rail-sweeper)

Rail Sweeper is a 3D first-person perspective rhythm game built using Unity and C#. The game was designed and built as a course project for "AI For Game Programming" at the University of Central Florida during the Fall 2024 semester. In Rail Sweeper you click floating notes to clear a path for the train you are riding on, and must also deal with "hold notes" that spawn directly on the track itself. All of this is done in perfect time with the song's beat.

During the project I programmed all of the game systems and implemented all of the visual and audio elements as well. Notes are spawned from an object pool to reduce the overall number of active game objects in the scene at any one time. The notes are spawned accurately using the Melanchall DryWetMIDI library, which reads note positions from a custom made MIDI file. In this manner the notes can be "played" on a regular keyboard while playing along to the song that was being implemented into the game. By using this method I avoided the need to manually set each note position in game. The notes in the MIDI file are quantized for better accuracy (locked to 1/16 notes for example), the BPM is set, and some simple math takes care of spawning the notes in the proper position in the game scene. This ensures that notes are always right on beat, as the song's current position in game is tracked in beats as well.

For added challenge a simple game AI was integrated that keeps track of the player's current "combo" score. The higher the player's combo, the further from their original spawn point and faster the note objects travel. Notes patterns are generated from a graph structure that holds various patterns (spirals, diagonals, zigzags), this prevents the notes from moving in random directions, and increase the game's playability.

During the project I designed and scripted the UI elements as well. Although simple, they are functional and provide a base level of polish necessary for player enjoyment. For example, when songs are completed at each difficulty, this data is saved in the player's game file and updated visually via a star that appears in the level selection menu. Player stats are also tracked for each level and displayed on completion of the song.





### Afterwords

###### MongoDB, Express, React, Node.js, TyhpeScript, JavaScript, Github

[Afterwords Website](http://copteam22.xyz/)

##### Repo
[Afterwords](https://github.com/Jsomerville1/cop4331largeproject)


Afterwords is a web and mobile app that allows users to send email messages and/or PDF files to designated persons if they fail to "check in" for a user defined period of time. For example, if the user does not check in to the app for 6 months, the messages are automatically sent to the user's recipients.

You may like to use the app to send a location of your hike if you haven't checked in for a few hours, for example. It can also be used to send messages or important files to loved ones upon death.

For this project I worked as the project manager, and delegated tasks to other team members. I also worked on API endpoints and some of the front end elements.



### Pirate Ships
###### Knight Hacks 2024
###### Python, pygame
<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/4wrOgf9LXGA?si=UjURjpdrk7r5Jm98" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<br>

Pirate Ships is an online multiplayer battleships clone. Two players play against each other in real time.

For this project I completed the primary game and server code using python and the pygame library. The server was hosted using a Google Cloud VM, and acts as a relay between the game clients on each player's computer.

##### Devpost
[Pirate Ships](https://devpost.com/software/pirateships)