## Warehouse Robot Pathfinding Simulator

An interactive warehouse robot pathfinding simulator built with React, Vite, and JavaScript. The project demonstrates how autonomous robots can navigate a grid-based warehouse using pathfinding algorithms, avoid obstacles, visualize routes, and process pickup tasks using a FIFO queue.

## Check it out here: https://ware-house-robot-path-finding.vercel.app/

## Features

- Interactive Warehouse Grid: Add or remove obstacles and customize the warehouse layout.
- Robot Navigation: Configure the starting point and destination.
- A Algorithm:* Find routes using heuristic-based search.
- Breadth-First Search (BFS): Explore nodes level by level.
- Depth-First Search (DFS): Explore paths through depth-first traversal.
- Algorithm Comparison: Compare supported pathfinding algorithms on the same grid.
- Path Visualization: Display explored cells and the calculated route.
- Robot Animation: Watch the simulated robot move along a route.
- Pickup Task Management: Add, remove, and clear pickup tasks.
- FIFO Task Queue: Demonstrate first-in, first-out task processing.
- Random Obstacles: Generate different warehouse scenarios.
- Performance Metrics: View the result metrics provided by the algorithms.
- Responsive Interface: Use the application on desktop and smaller screens.
 
## Tech Stack

- React
- Vite
- JavaScript
- JSX
- CSS
- A* Pathfinding
- Breadth-First Search
- Depth-First Search
- Queue and Priority Queue data structures

## Project Structure

warehouse-robot-pathfinding/
├── public/
│   └── robot.svg
├── src/
│   ├── algorithms/
│   │   ├── astar.js
│   │   ├── bfs.js
│   │   └── dfs.js
│   ├── components/
│   │   ├── ControlPanel.jsx
│   │   ├── MetricsPanel.jsx
│   │   ├── TaskManager.jsx
│   │   └── WarehouseGrid.jsx
│   ├── data-structures/
│   │   ├── PriorityQueue.js
│   │   └── Queue.js
│   ├── utils/
│   │   └── gridUtils.js
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
├── tests/
│   ├── pathfinding.test.js
│   └── setup.js
├── index.html
├── package.json
├── vite.config.js
├── eslint.config.js
├── README.md
└── documentation.md

## Installation and Setup

## Prerequisites

Install Node.js and npm on your computer.

# Clone the Repository

Replace "<your-github-username>" with your GitHub username.

git clone https://github.com/<your-github-username>/warehouse-robot-pathfinding.git
cd warehouse-robot-pathfinding

# Install Dependencies

npm install

Start the Development Server

npm run dev

Open the local URL displayed in the terminal, usually:

http://localhost:5173

Build for Production

npm run build

Preview the Production Build

npm run preview

The production build is generated in the "dist/" directory.

## How to Use

1. Open the application in your browser.
2. Select A*, BFS, or DFS from the algorithm controls.
3. Edit the warehouse grid by placing or removing obstacles.
4. Select a start cell and destination cell using the available editing controls.
5. Run the selected algorithm to calculate a route.
6. Use the algorithm comparison feature to compare search results.
7. Animate the robot to visualize its movement.
8. Add pickup tasks by entering a task name, row, and column.
9. Remove individual tasks or clear the queue when needed.
10. Run the pickup queue to process tasks in FIFO order.

The default internal start position is "{ row: 7, col: 3 }", and the default destination is "{ row: 7, col: 21 }". The interface displays coordinates starting from 1, while internal JavaScript grid indices start from 0.

## Algorithm Overview

# A* Search

A* combines the cost already incurred with a heuristic estimate of the remaining distance to guide its search.

# Breadth-First Search (BFS)

BFS explores neighboring nodes level by level. With equal movement costs, it finds a shortest path when a route exists.

#:Depth-First Search (DFS)

DFS explores one branch deeply before backtracking. It demonstrates graph traversal but does not generally guarantee the shortest path.

## Deployment

This project can be deployed to Vercel as a static Vite application.

1. Push the project to GitHub.
2. Sign in to "Vercel" (https://vercel.com/).
3. Import the GitHub repository.
4. Configure the following settings:

Setting| Value
Framework Preset| Vite
Root Directory| "./"
Install Command| "npm install"
Build Command| "npm run build"
Output Directory| "dist"

5. Click Deploy.
6. Open the generated URL and test the application.

## Testing

The project includes test-related files in the "tests/" directory. Check "package.json" for the configured testing framework and available test commands.

Before deployment, run:

npm run build

## Limitations

- The warehouse is a simulated grid environment.
- The robot does not control physical hardware.
- No live sensors or warehouse inventory systems are connected.
- Results depend on the selected algorithm and obstacle layout.
- Animation timing is for visualization and does not represent real-world robot speed.

## Future Enhancements

- Configurable pickup and delivery locations.
- Detailed mission-progress indicators.
- Step-by-step algorithm visualization.
- More detailed performance reports.
- Saved warehouse layouts.
- Additional automated tests.
- Optional integration with real-world warehouse data.

## License

No license is specified yet. Add a "LICENSE" file if you choose to distribute the project under an open-source license.
