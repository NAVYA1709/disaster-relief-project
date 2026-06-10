# Disaster Relief Resource Allocation System 🚑📦

An efficient, console-based disaster relief resource allocation system designed to identify the quickest supply delivery routes and manage priority queues, ensuring high-urgency zones receive life-saving resources first. 

By optimizing distribution routes during emergencies like floods and earthquakes, this system drastically reduces emergency response times and maximizes relief effectiveness.

---

## 🚀 Features

* **Shortest Path Optimization:** Employs Dijkstra's Algorithm to find the absolute fastest path between multiple relief centers and affected locations.
* **Dynamic Priority Queuing:** Processes high-urgency regions and nearest nodes first using an optimized Min-Heap structure.
* **Decoupled Data Architecture:** Leverages **Google Sheets** to organize, update, and manage locations, road connections, distances, and urgency levels seamlessly without code modifications.
* **Real-World Simulation:** Dynamically updates routes and simulates a live disaster distribution sequence upon execution.
* **Highly Scalable:** Handles complex, weighted terrain graphs efficiently via adjacency lists.

---

## 🛠️ Tech Stack & Core Logic

* **Language:** C++ 
* **Data Structures:** Graphs (Adjacency Lists), Priority Queue (Min-Heap)
* **Algorithms:** Dijkstra's Shortest Path Algorithm
* **Data Source:** Google Sheets (CSV/Structured format for input routing matrices)

---

## ⚙️ How It Works

1.  **Graph Construction:** The system reads location connections and road weights from the data source to construct an adjacency list.
2.  **Hub Isolation:** A source node (Relief Center) is designated.
3.  **Priority Evaluation:** The Min-Heap priority queue dynamically processes the closest nodes first while cross-checking location urgency metrics.
4.  **Route Relaxation:** Distances are dynamically calculated and updated across the map grid.
5.  **Output Deployment:** The final optimized paths, delivery sequence, and completion trackers are printed out for the log.


---

## 💻 Installation & Running the System

### Prerequisites
Make sure you have a modern compiler installed ($G++$ for C++ or $JDK$ for Java).

### Execution Instructions (C++)
```bash
# 1. Compile the source code
g++ main.cpp -o output

# 2. Run the executable program
./output
