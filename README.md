# Pathfinding Project

A Python toolkit for simulating smart GPS navigation in grid-based maps, supporting static and dynamic obstacles.


## Features

- **Map Support:** Easily switch between small, medium, large, and dynamic maps.
- **Dynamic Obstacles:** Vehicles and objects with deterministic or scheduled movement ([`DynamicObstacles`](src/obstacles.py)).
- **Extensible:** Add new search strategies or heuristics.
- **Unit Tests:** Coverage for grid loading and search algorithms.

## Project Structure

```
├── run.py                # Main entry point
├── requirements.txt      # Dependencies
├── src/
│   ├── grid.py           # Grid and map handling
│   ├── heuristics.py     # Heuristic functions
│   ├── localsearch.py    # Local search (future)
│   ├── obstacles.py      # Dynamic obstacle logic
│   ├── search.py         # BFS, UCS, A* implementations
│   └── utils.py          # Logging and utilities
├── maps/                 # Map files (static & dynamic)
├── tests/                # Unit tests
```


## Maps

- **Format:** First line: width height. Next lines: grid costs (`-1` for obstacles).
- **Dynamic obstacles:** See [`maps/dynamic.json`](maps/dynamic.json).


## Extending

- Add new heuristics in [`src/heuristics.py`](src/heuristics.py).
- Implement new search strategies in [`src/search.py`](src/search.py).
- Add new map files in [`maps/`](maps/).


Created by Suhana Bisht.
