# Autonomous Vehicle Management System (AVMS)

**Unit:** COMP1002 - Data Structures and Algorithms  
**Institution:** Curtin University Malaysia  
**Semester:** Semester 2, 2024  
**Project type:** Individual academic Java project  
**Portfolio format:** Documentation-only case study

## Overview

Designed and implemented an interactive Java-based system to model an autonomous vehicle fleet and a connected road network. The project applies custom abstract data types (ADTs) and data structures to manage city connections, vehicle records and vehicle recommendations.

This repository summarises the work described in the original technical report and manual test report. **Original Java source files are not included, and the application has not been recompiled or rerun for this portfolio.**

## Implemented components (as documented)

| Area | Implementation described in the technical report |
| --- | --- |
| Road network | Undirected graph with adjacency-list and adjacency-matrix representations; adding cities and roads; displaying neighbours and edges |
| Path checks | Recursive depth-first search (DFS) to determine whether a route exists between two locations |
| Vehicle registry | Custom linear-probing hash table with vehicle ID lookup, insertion, removal and resizing |
| Vehicle model | Java class for ID, make, model, location, destination, distance and battery level |
| Recommendations | Min-heap-based nearest-vehicle selection and Quicksort-based highest-battery selection |
| Interface | Interactive console menu for graph and vehicle operations, with input/error handling |

**Technologies:** Java, data structures and algorithms, graphs, DFS, hash tables, linear probing, heaps, Quicksort, object-oriented programming, console applications.

## Testing evidence

The original manual test document includes screenshots of adding roads and cities, checking graph paths and neighbours, creating/searching/deleting vehicle records, sorting by distance or battery level, and updating recommendations after deletion. See [Manual test evidence](docs/manual-testing.md).

These results reflect the **original report screenshots**, not independent testing performed for this GitHub package.

## Case study and limitations

- [Project design and implementation](docs/project-case-study.md)
- [Manual test evidence](docs/manual-testing.md)
- [Evidence, scope and publication notes](docs/verification-and-attribution.md)

**Sharing:** This is a summary of coursework rather than a reproduction of the submitted source or assessment handout. Keep this repository private until the applicable Curtin coursework-sharing requirements have been checked.
