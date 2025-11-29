⭐ A* Pathfinding Algorithm — Shortest Path on OpenStreetMap Data
📌 Overview

This project implements the A* (A-Star) search algorithm to compute the shortest path between two points on a map.
Using real-world OpenStreetMap (OSM) data, the algorithm finds an optimal route by combining the strengths of Dijkstra’s Algorithm and Greedy Best-First Search.

The project demonstrates how heuristic-based search improves efficiency in large road networks.

🚀 Features

Implements the A* shortest path algorithm from scratch

Uses heuristic + cost function to guide search efficiently

Works with OpenStreetMap XML road data

Visualizes the path and explored nodes

Modular and easy-to-understand C++ structure

Efficient handling of large map graphs

🧠 How A* Works

A* calculates the shortest path using the function:

f(n) = g(n) + h(n)


Where:

g(n) = cost from start node to current node

h(n) = heuristic estimate to the goal (Haversine distance)

f(n) = estimated total cost of the path through node n

This combination ensures the algorithm is both optimal and fast.

🛠️ Tech Stack
Component	Technology
Language	C++
Parsing	OpenStreetMap XML (.osm)
Build Tools	g++, Makefile
Visualization	(if included) PNG/SVG map drawing
📂 Project Structure (Typical)
/src
   ├── a_star.cpp
   ├── map_model.cpp
   ├── main.cpp
/osm_data
   └── <map>.osm
/CMakeLists.txt or Makefile

🔧 Setup & Compilation
1️⃣ Clone the repository
git clone https://github.com/your-username/a-star-osm.git
cd a-star-osm

2️⃣ Build the project

Using g++:

g++ -std=c++17 src/*.cpp -o a_star


Or using Makefile:

make

3️⃣ Run the program
./a_star


When prompted, enter:

start coordinates

end coordinates

path to the .osm map file

📊 Output

The program outputs:

The shortest path distance

Number of nodes explored

The final computed path

If visualization is included, it also generates:

A display window or image marking the path on the map

🌟 Example Use Case

Finding the shortest driving/walking route across:

A city map

A neighborhood

A road network graph

📈 Future Improvements

GUI-based map visualization

More heuristics (Manhattan, Octile)

Integration with real-time map tiles

Weighted edges for traffic conditions

Exporting paths as GPX/JSON

👥 Contributors

Bhoomija Garg

Kanishka Bhardwaj
