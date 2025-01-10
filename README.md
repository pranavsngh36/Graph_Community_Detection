# Graph Community Detection

This project analyzes the **CollegeMsg dataset**, a temporal network of messaging interactions among students at the University of California. The primary goal is to detect and analyze **communities of interactions** and explore their evolution over time using static and temporal network analysis techniques.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Tools and Libraries Used](#tools-and-libraries-used)
- [Future Work](#future-work)
- [Contact](#contact)

---

## Project Overview

The **Graph Community Detection** project is divided into two main phases:
1. **Static Analysis**: Examines the overall structure of the messaging network, treating all interactions as occurring simultaneously.
2. **Temporal Analysis**: Investigates the evolution of communities over different time intervals (hourly, 3-hour, and 6-hour slices).

Using **community detection algorithms** (e.g., Louvain), the project reveals how communities form, dissolve, and shift focus between academic and social contexts throughout the day.

---

## Features

- Constructs static and temporal graphs from the dataset.
- Detects communities using the **Louvain algorithm** and calculates modularity scores.
- Filters graphs based on node degree thresholds to focus on influential participants.
- Analyzes and visualizes community dynamics over different time intervals.
- Tracks node evolution to understand the roles of key individuals in the network.
- Provides visualizations of community structures and modularity over time.

---

## Dataset

The dataset used is the **CollegeMsg dataset** from Stanford University's SNAP repository. It contains:
- **Sender**: ID of the user sending the message.
- **Receiver**: ID of the user receiving the message.
- **Timestamp**: Unix timestamp of when the message was sent.

---

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/Graph-Community-Detection.git
cd Graph-Community-Detection
```

2. Install the required libraries:
```bash
pip install networkx python-louvain matplotlib pandas
```
3. Ensure the CollegeMsg dataset is available in the project directory.


## Usage

### Static Analysis
Run the first part script to perform static analysis.
- Constructs the network graph.
- Applies the Louvain algorithm to detect communities.
- Filters high-degree nodes and visualizes subgraphs.

### Temporal Analysis
Run the second Part script  to perform temporal analysis.
- Divides the dataset into hourly, 3-hour, and 6-hour intervals.
- Applies the Louvain algorithm to each time slice.
- Visualizes modularity scores and community evolution.


## Result

### Static Analysis
- Number of nodes: X
- Number of edges: Y
- Number of detected communities: N
- Modularity score: 0.XXX

### Temporal Analysis
- Hourly Modularity: Scores vary from X to Y.
- 3-Hour Modularity: Scores highlight trends of increasing social interaction in the evening.
- Morning vs Evening: Communities shift from academic to social clusters throughout the day.

### Visualizations include:

- Static community structure.
- Temporal community evolution at different intervals.
- Modularity scores over time.

## Tools and Libraries Used

- Python
- NetworkX: For graph construction and analysis.
- Matplotlib: For visualization of graphs and modularity scores.
- Pandas: For data manipulation and preprocessing.
- Community-Louvain: For modularity-based community detection.

## Future Work

- **Predictive Modeling**: Develop forecasting models to predict future interactions.
- **Dynamic Community Detection**: Implement advanced temporal community detection algorithms.
- **Interactive Visualizations**: Use tools like Plotly or Gephi for interactive graph analysis.

## Contact

For any questions or contributions, please contact:

- Name: Pranav Singh
- Email: pranavsngh36@gmail.com
- GitHub: https://github.com/pranavsngh36