https://www.tryexponent.com/blog/system-design-interview-guide
A system design interview is usually composed of 5 steps:

Step 1: Understand the problem. Get to know the problem by asking questions and define the scope and constraints of the design.
What are the functional (features the system should offer) and non-functional (speed, consistency, security,etc) requirements for the system's design?
What is included and excluded from this design?
Who are the clients/consumers?

Consider these questions to identify the non-functional requirements:
What is the scale of the system?
How many users should the application support?
How many requests should the server handle?
Are most use cases read-only?


Step 2: Design the system.  Outline the most essential parts of the system and show how they work together to achieve the desired function. 
START DESIGNING APIs (REST/RPC/GRAPHQL) WITH ITS REQUEST PARAMETERS AND RESPONSES. 
DATA MODELING: Simple schema that lists most important fields, Discuss data access patterns and read-write ratio, Discuss indexing, and which database to use

Step 3: Explore the design. You or your interviewer will choose an interesting component and discuss its details.
Consider how non-functional requirements impact design choices.
Transactions: If the system requires transactions, consider a database that offers the ACID
Data size, Partitioning, Offline processing, etc

Step 4: Improve the design: Bottlenecks and Scale
Single points of failure: How could the system be more robust and maintain uptime?
Data replication: Is the data important enough to make copies? How important is it to keep all copies the same?
CDNs: Does it provide a service for people all over the world? Would data centers in different parts of the world make it faster?

Step 5: Wrap up. Check that the design meets all requirements and suggest ways to improve it.

![image](https://github.com/DanielJulian/entrevistas/assets/21090149/46ac8ff7-cca9-4deb-8a53-9751fa001669)





Horizontal vs Vertical Scaling
Horizontal scaling refers to increasing the capacity by adding additional machines. -> Harder to maintain, but improves fault tolerance.
Vertical scaling refers to increasing the resources of existing machines. -> Easier to maintain, but there is a limit to it, and also there is a single point of failure
