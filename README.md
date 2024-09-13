---

# Bird Tracking Data Analysis

This project analyzes bird migration patterns using longitude and latitude data for multiple bird species. The data is visualized through graphs and maps to study the flight trajectories of the birds. The project primarily focuses on the movement of a bird named "Eric" and compares the flight paths of different birds using various visualization techniques.

## Table of Contents
- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Visualization](#visualization)
  - [Individual Bird Tracking](#individual-bird-tracking)
  - [Multiple Bird Trajectories](#multiple-bird-trajectories)
  - [Map Plotting](#map-plotting)
- [Class Definition](#class-definition)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction

This project uses bird tracking data to visualize the flight paths of various birds. It demonstrates data handling and visualization using Python libraries such as Pandas, Matplotlib, and Cartopy. The data provided includes the bird names, their longitudes, and latitudes at different points in time.

## Technologies Used
- Python 3.x
- Pandas
- Matplotlib
- NumPy
- Cartopy (for map plotting)

## Installation

1. Clone the repository or download the project files.
2. Install the required libraries:
   ```bash
   pip install pandas matplotlib numpy cartopy
   ```

## How to Run

1. Load the bird tracking data (`bird_tracking.csv`) into the project using Pandas.
2. Run the provided code to visualize the bird migration patterns on a scatter plot and a map.

## Visualization

### Individual Bird Tracking

The project tracks the movements of a specific bird, "Eric," by plotting his longitude and latitude data on a scatter plot.

### Multiple Bird Trajectories

A for-loop is used to plot the trajectories of all birds on the same graph, with different colors representing different birds.

### Map Plotting

Using the Cartopy library, the project plots bird trajectories on a geographical map, showcasing their migration over land, sea, and country borders.

## Class Definition

A custom class `Geodic` is defined to store the name of the birds and provide a structured way to represent individual bird data.

```python
class Geodic:
    def __init__(self, name):
        self.name = name

    def __repr__(self):
        return f"Geodic({self.name!r})"

# Example usage:
geodic = Geodic("Eric")
print(geodic)
```

## Conclusion

This project offers a simple and visual way to study bird migration patterns using Python data analysis and visualization libraries. The use of Cartopy adds an additional layer of geographic context to the flight paths of the birds.

---
