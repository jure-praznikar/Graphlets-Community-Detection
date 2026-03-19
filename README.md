# Graphlets-Community-Detection

A method for community detection in graphs using graphlet-based adjacency matrices combined with the FastGreedy algorithm.

## Overview
For each graphlet orbit (G0–G8), the corresponding adjacency matrix is computed using [GRADCO]. Each graphlet matrix is normalized and added to the baseline adjacency matrix (G0). Community detection is then applied using the FastGreedy algorithm (via igraph), and results are evaluated using NMI, ARI, and Modularity.

## Project Structure
```
example_1.ipynb # Main notebook with the full pipeline
requirements.txt # Python dependencies
graphlets/ # Output folder for graphlet adjacency matrices (G0–G8)
final_results.csv # Output: community detection metrics per graphlet
```

## Requirements
Install dependencies with:

```bash
pip install -r requirements.txt
```

## Usage
1. Open `example_1.ipynb` in Jupyter or VS Code.
2. Run all cells in order.
3. Results are saved to `final_results.csv`.

## Metrics
| Metric | Description |
|--------|-------------|
| NMI | Normalized Mutual Information |
| ARI | Adjusted Rand Index |
| Modularity | Quality of the detected community structure |
