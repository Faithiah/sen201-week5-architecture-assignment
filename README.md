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
