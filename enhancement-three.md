# Enhancement Three - Databases

### The image links to the repository

[![Enhancement Three](https://i.postimg.cc/vZcFG453/Screenshot-2025-10-18-110537.png)](https://github.com/karina-42/elChupacabras)

## Narrative

Briefly describe the artifact. What is it? When was it created?

I used the same artifact I used in Enhancement One and Two, the text-based game written in Python, created in IT 140. In Enhancement One, I refactored the code into an object-oriented design and added a replay feature. In Enhancement Two, I organized the rooms into a graph data structure and used a Breadth First Search (BFS) algorithm to implement a hints feature that tells the player how to get to the closest room with an item.

Justify the inclusion of the artifact in your ePortfolio. Why did you select this item? What specific components of the artifact showcase your skills and abilities in software development? How was the artifact improved?

The original artifact was a simple game played in the console, without a database, user authentication, or user interface. The enhanced artifact included in my portfolio demonstrates my ability to refactor a console-based application to a full stack application with many new features. In addition to replaying the game upon finishing it and getting hints when they need it, players can also see a scoreboard of their best times completing the game. They can create a user profile and use it to log in to play and save their scores. The passwords they created are hashed to ensure privacy and safety. The classes are in separate files, making the code modular.

Did you meet the course outcomes you planned to meet with this enhancement in Module One? Do you have any updates to your outcome-coverage plans?

I planned to meet outcome 1: “Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science.”, outcome 4: “Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals.”, and outcome 5: “Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources.”
I met outcome 1 by building a web app with Flask that allows multiple users to register and log in to interact with the game. I accomplished this by implementing user authentication, which also shows I met outcome 5. Other ways I incorporated security include using password hashing, validation, try/except blocks, and preventing SQL injection attacks by using SQLAlchemy. Using Python classes, Flask, SQLAlchemy, and Jinja templates shows I met outcome 4, as I used several tools to accomplish my goal of creating a full stack application.

Reflect on the process of enhancing and modifying the artifact. What did you learn as you were creating it and improving it? What challenges did you face?

Although I had experience making full stack apps with JavaScript, MongoDB, Express, and NextJs, this was my first time creating a full stack app with a Python stack. I started by following a tutorial that created a full stack Python app using Flask and SQL, similar to what I had planned to do. I did not follow it exactly, as I implemented changes and enhancements to align with my plans for my application, such as using try/except blocks to catch exceptions, adding a Scoreboard page, and styling the home page to fit my text-based game. I did this by referencing the documentation available. My experience in creating full stack apps in JavaScript stack helped me in my goal of creating a full stack Python app. I refreshed my backend knowledge and got some experience using Jinja as a templating language to dynamically update the text as the player plays. Along the way, I refactored the main.py file by breaking each class into its own file to make the project more modular.
Implementing the Scoreboard proved challenging at first, but I began by creating a Python function in the Game class to get the time the player started and ended, then calculated the time elapsed. Using print() to debug, I determined when the time was being saved and calculated and that helped to figure out where to call the function. To make the code clearer, I then separated it into two functions, one to get the starting time and another to get the ending time and calculate the elapsed time.
