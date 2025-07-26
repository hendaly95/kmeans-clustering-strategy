# 📊 K-Means Clustering Strategy Project

This project implements and evaluates two different strategies for selecting initial cluster centers in the K-Means clustering algorithm. It is part of the coursework for **CSE 575: Statistical Machine Learning**.

## 🧠 Project Goals

- Implement K-Means from scratch in Python.
- Evaluate the effect of initialization strategies on clustering loss.
- Compare clustering quality across multiple cluster counts (k = 2 to 10).
- Visualize the resulting clusters and performance metrics.

## 📁 Project Structure

| File                 | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `project2_part1.ipynb` | K-Means implementation with random initialization (Strategy 1)             |
| `project2_part2.ipynb` | K-Means implementation with distance-maximizing initialization (Strategy 2)|
| `precode.py`         | Preprocessing and helper functions used in both notebooks                   |
| `Project-Part 1.pdf` | Report and analysis for Strategy 1                                          |
| `Project-Part 2.pdf` | Report and analysis for Strategy 2                                          |
| `Project Description.pdf` | Full overview of project requirements and objectives                    |

## 🔍 Strategies

### 🧪 Strategy 1: Random Initialization
- Randomly selects k initial centers from the dataset.
- Repeats for cluster sizes k = 2 through 10.
- Computes and records the loss for each k.

### 🧬 Strategy 2: Distance-Maximizing Initialization
- First center is chosen randomly.
- Subsequent centers are selected based on maximizing average distance from all previously chosen centers.
- Tested for k = 2 to 10 with corresponding loss evaluations.

## 📈 Outputs

For each part:
- Final centroid coordinates for each k.
- Loss values across all cluster counts.
- Plots of loss vs. number of clusters.
- Cluster visualizations (2D scatter plots).

## 🛠️ How to Run

1. Install necessary packages:
```bash
pip install numpy matplotlib
```

2. Run `project2_part1.ipynb` to evaluate Strategy 1.
3. Run `project2_part2.ipynb` to evaluate Strategy 2.

Each notebook will output:
- Final centroids in format:  
  ```
  [[x1, y1], [x2, y2], ..., [xk, yk]]
  ```
- Loss values in format:  
  ```
  L1, L2, ..., L9
  ```

## ⚠️ Notes

- This project uses a provided `.npy` dataset (`AllSamples.npy`) containing 2D points, which is **not included** in this repository.
- You must supply or generate your own compatible dataset to rerun the project.
