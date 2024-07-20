# IslandNetwork Traffic Modelling Tool

## Project Overview

The Traffic Congestion Modeling Tool is a Java-based simulator designed to analyze and predict traffic flows and congestion in city networks. It computes the optimal paths and traffic capacities between cities using sophisticated algorithms. This tool is invaluable for urban planning and congestion management.

## Key Features

- Maximum Flow Calculation: Utilizes Depth First Search (DFS) and the Ford-Fulkerson method to determine the maximum number of cars that can traverse between two cities without exceeding road capacities.
- Shortest Path Determination: Implements Dijkstra’s Algorithm to find the most efficient routes between cities, minimizing travel time and congestion.

## Dependencies
 Java Development Kit (JDK 11 or later) <br>
 Apache Maven (3.6.3 or later) <br>

 ## Installation
 Clone the repo
 ```bash
 git clone https://github.com/vinitvala/IslandNetwork
 ```

## Usage
This tool requires a list of cities and roads with specified carrying capacities (cars per minute). Execute the simulator through the command line to analyze traffic flow and determine efficient routing and capacity handling across the network.

## Sample Execution
Upon launching the application, users are greeted with the following interface:

Welcome to the Island Network!
```bash
please enter an url:
```

```bash
Map loaded.

Cities:     //Alphabetical Order
---------------------
Bones Beach
Composting Fields
Fire Hazard
Fishingville
Gatsby
Kingkongoma
Lawn City
North Spoon
Small Pear
South Spoon
Stream Foot
University

Road                                  Capacity
----------------------------------------------
Composting Fields to Small Pear            12
Lawn City to Small Pear                    30
Hipster to Small Pear                      14
Hipster to Small Pear                      16
Lawn City to Hipster                       16
Gatsby to Composting Fields                10
Fishingville to Lawn City                  17
Fishingville to Gatsby                     11
Bones Beach to Hipster                     12
Bones Beach to Lawn City     	            8
Fire Hazard to Bones Beach                 13
Kingkongoma to Fire Hazard                  7
Kingkongoma to Lawn City                   20
University to Kingkongoma                   6
University to Fishingville                 18
Stream Foot to University                   6
Steam Foot to Kingkongoma                  11
North Spoon to Stream Foot                 15
South Spoon to Stream Foot                 20

Menu:
    D) Destinations reachable (Depth First Search)
    F) Maximum Flow
    S) Shortest Path 
    Q) Quit
    
Please select an option: D
Please enter a starting city: University
DFS Starting From University:
Fishingville, Gatsby, Composting Fields, Small Pear, Lawn City, Hipster, Kingkongoma, Fire Hazard, BonesBeach
Please select an option: D
Please enter a starting node: South Spoon
DFS results (destinations reachable):
Stream Foot, Kingkongoma, Lawn City, Small Pear, Fire Hazard, Bones Beach, Hipster, Fishingville, Gatsby, Composting Fields
Please select an option: F
Please enter a starting city: University
Please enter a destination: Hipster
Routing: 
University->Fishingville->Lawn City->Hipster: 16
University->Kingkongoma->Fire Hazard->Bones Beach->Hipster: 6
Maximum Flow: 22
Please select an option: F
Please enter a starting city: University
Please enter a destination: South Spoon
No route available!
Please select an option: S 
Please enter a starting node: Kingkongoma
Please enter a destination node: Small Pear
Path: Kingkongoma->Fire Hazard->Bones Beach->Hipster->Small Pear
Cost: 46
Please select an option: Q

Goodbye!

```

This README provides a comprehensive guide to setting up and utilizing the Island Network Tool for effective traffic management in urban settings.


