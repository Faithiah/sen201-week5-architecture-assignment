# sen201-week5-architecture-assignment
week-5-assignment 
## CLIENT SERVER 
Client–Server architecture is a software design style where a system is divided into two main parts:
Client: The part that requests services (e.g., a browser, mobile app)
Server: The part that provides services (e.g., database server, web server)
The client sends requests over a network, and the server processes those requests and sends back responses.
## MAJOR COMPONENTS 
1. Client
Sends requests to server
Displays results to user
Handles user interaction (UI/UX)
2. Network
Transfers data between client and server
Uses communication protocols (HTTP, TCP/IP)
3. Server (Application Server)
Processes client requests
Runs business logic
Controls system operations
4. Database Server
Stores and manages data
Handles queries from the server
Ensures data integrity and security
## SIGNIFICANT ARCHITECTURAL DESIGN 
 1. Centralized vs Distributed Servers
Decision: Use one server or multiple servers
Rationale:
Single server is simple but risky
Multiple servers improve scalability and reliability
2. Stateless vs Stateful Communication
Decision: Whether server remembers client sessions
Rationale:
Stateless (e.g., HTTP) improves scalability
Stateful improves user experience but increases complexity
3. Thick Client vs Thin Client
Decision: Where to place most of the processing
Rationale:
Thin client → server does most work (easy to maintain)
Thick client → client handles more logic (better performance, less server load)
## SIGNIFICANT TRADE-OFFS OR CHALLENGES 
1. Single Point of Failure
In a typical client-server system, the server is central.
If the server crashes → all clients are affected
System availability depends heavily on server uptime
Example:
If your backend server goes down, your mobile/web app becomes unusable.
Implication:
You must implement:
Redundancy (backup servers)
Fail over mechanisms
2. Scalability Challenges
As users increase, the server can become overloaded.
Too many client requests → slow response time
Requires more resources (CPU, RAM, bandwidth)
Solution approaches:
Load balancing
Horizontal scaling (multiple servers)
Caching frequently requested data
3. Network Dependency & Latency
Client-server systems rely heavily on network communication.
Poor internet → slow system performance
High latency affects user experience
Example:
A user in a low-network area may experience delays when fetching data from the server.
## AREAS WITHIN CLIENT SEVER 
Pattern 1: Model-View-Controller (MVC)
What it is:
MVC separates your system into three parts:
Model → Data & business logic (usually on the server)
View → UI (client side)
Controller → Handles input & communication
How it fits Client-Server:
Client (View) → Displays data
Server (Model + Controller) → Processes and returns data
Why it is useful:
Clean separation of concerns
Easier maintenance
Allows frontend and backend to evolve independently
Pattern 2: Singleton Pattern
What it is:
Ensures a class has only one instance and provides a global access point.
Where to use it in Client-Server:
Database connection manager
Server configuration manager
Why it is useful:
Prevents multiple unnecessary connections
Saves system resources
Ensures consistency
 
  echo "Instructor/Peer Review: Evaluate README.md for completeness, justification, and adherence to design principles." git add .
  git commit -m"added CLIENT SEVER"
  git push
  
