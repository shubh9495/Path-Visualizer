Path visualizer is a Java-based mapping application that calculates and visualizes routes between geographic points using classical graph algorithms. this project demonstrates real-world graph theory applications via an interactive map interface powered by the Google Maps API.

## Features

- Compute shortest paths using Breadth-First Search (BFS), Dijkstra’s Algorithm, and A* Search
- Interactive route visualization on Google Maps
- Real-world road data integration with Java and JavaFX frontend

---

## About the Project

This project emphasizes algorithmic problem-solving through route planning, integrating backend graph logic with a frontend Google Maps interface. It’s a simplified but educational alternative to commercial mapping systems, focusing on algorithm design over production-grade UX.

### Learning Objectives

- Implement graph structures and traversal algorithms from scratch in Java
- Understand trade-offs between different shortest path algorithms
- Visualize algorithm performance and pathfinding behavior in real geographic contexts

---

## Getting Started

### Prerequisites

- **Java 8 or higher** – [Download here](https://www.oracle.com/java/technologies/javase-downloads.html)
- **Maven** – Dependency and build manager ([Install guide](https://maven.apache.org/install.html))
- **Google Maps API Key** – Get one [here](https://developers.google.com/maps/documentation/javascript/get-api-key)
- **Eclipse IDE** (optional) – or use any Java IDE of your choice

### Installation

1. **Clone the repository**
   ```bash
  
   ```

2. **Navigate to the project directory**
   ```bash
   cd UCSDGraphs
   ```

3. **Set your Google Maps API key**

   Create the following file if it doesn't exist:
   ```properties
   # File: src/main/resources/config.properties
   google.maps.api.key=YOUR_API_KEY
   ```

4. **Build the project**
   ```bash
   mvn clean install
   ```

### Running the Application

1. Launch the JavaFX application:
   ```bash
   java -jar target/UCSDGraphs-1.0-SNAPSHOT.jar
   ```

2. Open `http://localhost:8080` in your browser to interact with the map interface.

---

## Implementation Highlights

### 1. **Graph Structure & Node Design**

Custom `MapGraph` class represents the map:
- Nodes: `GeographicPoint` intersections
- Edges: directed, weighted road segments