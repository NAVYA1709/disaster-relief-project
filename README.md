# disaster-relief-project
An efficient disaster relief resource allocation system to identify the quickest delivery routes and priority queues to ensure that high-urgency  areas receive supplies first. The system seeks to optimize resource distribution during  emergencies like floods and earthquakes, thereby reducing response time and maximizing relief  effectiveness.
How to run
1. Compile the code
g++ main.cpp -o output
2. Run the program
./output

(For Java, replace with javac and java commands)

Project Overview

A console-based system that simulates disaster relief management using graph algorithms.

It calculates the shortest and most efficient routes between locations to ensure fast delivery of resources during emergencies.

Core Logic
Graph representation of locations
Priority Queue (Min Heap) for optimization
Dijkstra’s Algorithm for shortest path calculation
Features
Finds shortest path between multiple locations
Optimizes resource distribution routes
Handles weighted graphs efficiently
Fast computation using priority queue
Simulates real-world disaster response scenarios
Input / Output
Input
Number of nodes (locations)
Edges with distances (roads)
Source node
Output
Shortest distance from source:
Node 1 → 0
Node 2 → 4
Node 3 → 7
Node 4 → 9
File Overview
main.cpp        — Core implementation (Dijkstra + Priority Queue)

(Adjust if you have multiple files)

How it works
Graph is created using adjacency list
Source node is selected
Priority queue processes nearest node first
Distances are updated dynamically
Final shortest paths are printed

Limitations
No graphical interface
Static input (manual input required)
No real-time data integration
Future Improvements
Integrate Google Maps API for real-world routing
Add GUI (web or app interface)
Store data using database (Firebase)
Real-time disaster tracking
Tech Stack
Language: C++ / Java
Data Structures: Graphs, Priority Queue
Algorithm: Dijkstra
