---
title: Projects
excerpt: "Projects"
aside: false
---

### Army Reserve Mercury
###### React Native, AWS (Lambda, S3, API Gateway, RDS), Python, PostgreSQL, JavaScript

Army Reserve Mercury is a mobile and web application that streamlines administrative processes for Army Reserve soldiers and leaders. Reserve Mercury served as my senior design project where I led a team of 11 developers to introduce three new features, a multitude of bug fixes, and backend improvements to make the application more stable and useful to its end users. During my year on the project, I also completed a paid summer fellowship program in which I worked with 5 other developers full time on the application.

Below I will list my accomplishments during the senior design project and the fellowhsip:

##### Senior Design

During my time as project manager for Reserve Mercury's senior design semesters (Spring and Fall 2025) we delivered three new features. These included the RST Utilization page, form field highlighting for pay forms returned for correction, as well as a form audit log, and a guided user tutorial with separate tutorial flows for leaders, pay admins, and soldiers. I also created a series of tutorial videos for leaders, for pay admins, and for soldiers. These videos are a guide for new or returning users to get up to speed with how the application works and the different features available to the users. 

###### RST Utilization

The RST Utilization page tracks RST forms, or rescheduled training forms, and is accessible by Army Reserve leaders to track which soldiers have submitted RST forms for each battle assembly date (BA Date). The leader can select different units if they are in charge of multiple, and then select a specific BA Date to view. This shows a list of every soldier in the unit, whether or not they have an RST submitted for that date, and how many RSTs they have submitted for the fiscal year. The leader can also select any solider from the list to view all of that soldiers RST forms as well as the status of these forms. These features make it easy to quickly see which soldiers and how many of them will be absent from an upcoming battle assembly. The submitted makeup days are also viewable with the RST Utiliztion page.

###### Form Field Highlights and Audit Log

A pay form for Reserve soldiers goes through multiple processes before it is considered fully approved. The final step is for a pay administrator to check the form over and approve it, unless they find an error in the form. Prior to this new feature it could be confusing for a leader to have approved a form which later is denied by a pay admin and resubmitted by the soldier. This led to the approver questioning why the form was back in their approval queue. The new form audit logs tracks all approvals, denials, and resubmissions. This way the approver knows that the form has already been approved and is simply being resubmitted.

The other portion of this new feature is form field highlighting. When a form is deneid by a pay administator, the admin can now select which field on the pay form has the error, and leave a comment about what specifically needs correction. Then when the soldier opens the form to correct it, the field is highlighted and the comment is easily viewable so that they know at a glance what needs to be fixed.

###### User Tutorial

These interactive click-through tutorials appear for every new user on their first login, or for any user that has not completed them yet. The user has the option to skip the tutorial, click through with the "Next" and "Back" buttons, or follow each instruction in the actual application, which auto advances the tutorial as the user completes each step.

Multiple click-through tutorials were created such that there are separate guides for enlisted soldiers, leaders, and pay administators. This way each user gets a customized interactive guide for their specific use case. The user's tutorial status is tracked with a column in the users table that tracks whether the user has seen the mobile and web versions of the tutorial. Completing the tutorial or selecting the do not show option trigger the status such that the pop up is no longer displayed for that user.

#### Defense Innovation Fellowship

During the summer fellowship my duties included multiple bug fixes and the AFTP Utilziation feature, which I engineered from mockup to full implemented feature in the front and back end, and on both the mobile and web versions of the application. The AFTP Utilization feature tracks flight data for flight units in the Army Reserve. This is critical information for leaders of these units, as this data is at times the subject of aduits, and ensuring that it is accurate is very important.

The tool implements a few different features. Leaders can select any unit that they have access to, which provides a table of every solider in the unit. Each soldier's flight statisics are displayed, including the number of AFTP (Additional Flying Training Period) forms submitted for the fiscal year, the number of forms approved, and the number of forms paid. If there is a discrepancy between the number of forms stored in the database and the soldier's current "AFTP Number", then a warning is displayed, and the leader can select that solider to view more information.

A list is then displayed of all of the soldiers AFTP forms by AFTP number. Any missing forms are highlighted in red, and the leader can then manually enter that form if they have the paper copy, ensuring that the data stored in the application is accurate for audit purposes.




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