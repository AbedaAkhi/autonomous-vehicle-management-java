# Case Study - Autonomous Vehicle Management System

## Problem and scope

The COMP1002 assignment was to create an Autonomous Vehicle Management System (AVMS) using data structures and algorithms rather than relying solely on standard collections. The solution was documented in a 24-page individual technical report submitted in November 2024.

The application models a road network of cities, stores vehicles identified by unique IDs, and supports queries and recommendations through an interactive text menu.

## Road-network graph

- Represented a road network with both an adjacency matrix (edge distances) and an adjacency list (neighbour connections).
- Used custom `DSADoublyLinkedList` and `DSAGraphVertex` components to represent connected locations.
- Added and displayed cities and undirected roads, retrieved neighbours, and rejected attempts to connect locations not found in the graph.
- Implemented `isPath` using recursive depth-first search (DFS) with a visited-state check.

## Vehicle registry and data model

- Created a `Vehicle` model with a unique vehicle ID, make, model, current location, destination, distance to destination and battery level.
- Used a `VehicleHashTable` backed by a custom linear-probing hash table to add, find and remove vehicle records.
- Documented duplicate vehicle-ID handling, missing-record handling and hash-table resizing/rehashing.

## Sorting and recommendations

- Used a heap/min-heap approach to order vehicle distances and find the nearest vehicle.
- Used Quicksort to order vehicles by remaining battery level and identify the vehicle with the highest battery level.
- Rebuilt the heap structures after vehicle removal to keep the recommendation lists consistent with current records.

## Console interface

The interactive menu covered city/road insertion, graph viewing, path and neighbour checks, vehicle insertion/deletion/search/display, sorting by distance and battery, and nearest/highest-battery recommendations. The report also documents input validation and error messages.

## Challenges documented in the report

The technical report describes creating a graph edge representation for weighted city connections and adding a min-heap implementation because the existing practical-work heap was a max heap. It includes UML-style class diagrams and discussion of data-structure choices.

## Technical scope

This is an educational command-line system. It does **not** establish real-world vehicle autonomy, live GPS tracking, production dispatch, or integration with physical vehicles.

## Portfolio accuracy

The original Java source files were not supplied with this portfolio request. This case study describes the code and screenshot evidence present in the submitted report; independent compilation and live testing were not possible.
