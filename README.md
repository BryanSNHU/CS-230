# CS-230

# Briefly summarize The Gaming Room client and their software requirements. Who was the client? What type of software did they want you to design?
	The Gaming Room client wanted me to develop a web-based game from their already established Android version of Draw It or Lose It. The object was to form a scalable backend that handles multiple teams using different platforms, like a computer and a mobile device that hands inputs on the cloud while the local device handles the display and UI formats.


# What did you do particularly well in developing this documentation?
	I believe using the Object-oriented programming principles was well iterated, applying the Singleton pattern to manage the game service and the Iterator pattern for entity validation. The use of a base Entity class to handle shared attributes like id and name demonstrates a strong grasp of the DRY (Don't Repeat Yourself) principle and inheritance.

# What about the process of working through a design document did you find helpful when developing the code?
	The UML Domain Model clarifies the one-to-many relationships between the GameService, Game, Team, and Player, which serves as a blueprint for data structures.

# If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
	If I were to go back and revise my work, I would want to understand and explain the system architecture view. It was not a requirement, but adding some detail showing how a server stored data for a returning user.

# How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?
	By making the game more accessible to people, we eliminated the need for on device power when shifting the game to a web client. This was achieved by designing a backend that accounts for network latency and utilizes responsive web design for various screen sizes. Considering user needs is critical because it dictates the technical requirements. For example, failing to account for connection drops would lead to a poor user experience; thus, implementing robust retry logic was essential to satisfy the need for seamless gameplay.

# How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?
	My approach centered on encapsulation and memory management. By keeping member variables private and using a Singleton, you ensured the internal state of the game remains secure and controlled. In the future, some strategies I would use is pairing a relational database such as MySQL, for persistent data with an in-memory store (Redis) for high-speed session management to minimize latency. incorporating HTTPS/TLS encryption and strong password hashing from the initial design phase to protect user data would also be strategies to incorporate for a web game like draw it or lose it.
  
