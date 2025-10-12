# Enhancement Two - Algorithms and Data Structures

### The image links to the repository

[![Enhancement Two](https://i.postimg.cc/jddQVw9K/Screenshot-2025-10-12-162256.png)](https://github.com/karina-42/elChupacabrasEnhancementTwo/tree/main)

## Narrative

Briefly describe the artifact. What is it? When was it created?

I used the same artifact I used in Enhancement One, the text-based game written in Python, created in IT 140. In Enhancement One, I refactored the code into an object-oriented design and added a replay feature. This is the version that I further enhanced in Enhancement Two.

Justify the inclusion of the artifact in your ePortfolio. Why did you select this item? What specific components of the artifact showcase your skills and abilities in software development? How was the artifact improved?

In the original artifact, players play the game without a map or any knowledge of the rooms and items they need to win the game. This encourages replayability to become familiar with the paths, rooms, and items, but can also result in frustration if players keep losing. I thought introducing a hints feature might help players if they cannot find a room with an item.
To solve this problem, I first turned the rooms dictionary into a graph data structure with a new GraphFactory class. I opted to use the factory pattern again for scalability, as it could be used in the future to add more rooms, connections, or even other houses and buildings. At the moment, more rooms can be added by simply adding the data to the rooms_config dictionary, making sure to also update the “exits” of connected rooms. This demonstrates my ability to refactor code with attention to scalability and maintainability. 
My next step after this was to use a breadth-first search (BFS) algorithm to implement the hints feature. I wanted the hint to be a path from the player’s current room to the closest room with an object. Since BFS returns the shortest path, I thought it would be the perfect fit. The rooms represented the nodes of the graph, and the directions to the rooms represented the edges. Using the Room.has_item method I created in the first enhancement, BFS traversed the rooms until it found a room with an item, then returned the path it took to the player. This demonstrates my ability to create reusable methods, problem solving abilities, and picking appropriate algorithmic solutions.

Did you meet the course outcomes you planned to meet with this enhancement in Module One? Do you have any updates to your outcome-coverage plans?

I planned to meet outcome 2: “Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts”, outcome 3: “Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices.”, and outcome 4: “Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals”.
I met outcome 2 by once again documenting my code with docstrings and comments, updating docstrings from the first enhancement to incorporate the changes of the second enhancement, and using descriptive names for classes, methods, and variables. I met outcomes 3 and 4 by researching and applying the Factory pattern to create the graph data structures and the BFS algorithm to solve the problem I was facing using appropriate tools and techniques. 

Reflect on the process of enhancing and modifying the artifact. What did you learn as you were creating it and improving it? What challenges did you face?

When I first created the artifact, I had little experience with algorithms, complex data structures, or design patterns. Through these enhancements I am learning not only the theory behind these topics but also practical implementations. Realizing that the Room.has_item() method I had written in the first enhancement could easily be reused in the BFS algorithm to find a room with an item showed me the importance of writing modular, reusable code. One of the biggest challenges I faced was juggling dictionaries, lists, and objects, making it difficult to remember when to use dot notation, square brackets, or methods like .get(), .items(), or .values() to access data. I made liberal use of print statements for debugging and eventually developed a personal cheatsheet to help me.
