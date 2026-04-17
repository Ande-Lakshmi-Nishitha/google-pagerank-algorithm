# Google PageRank Algorithm

This project implements the **PageRank algorithm**, originally developed by Google to rank web pages based on their importance in a network of links.

---

## Overview

The PageRank algorithm is a link analysis algorithm used to measure the importance of nodes (web pages) in a graph. It assigns a numerical score to each node based on incoming links and their respective importance.

Pages with more high-quality incoming links receive higher rankings.

---

## Key Concepts

* Graph Representation
  Web pages are represented as nodes, and hyperlinks as directed edges.

* Random Surfer Model
  A user randomly clicks links, occasionally jumping to any page (damping factor).

* Damping Factor (d)
  Typically set to `0.85`, representing the probability of following a link.

* Iterative Convergence
  PageRank values are updated repeatedly until they stabilize.

---

## Features

* Implementation of PageRank algorithm
* Handles directed graphs
* Supports iterative computation
* Demonstrates convergence behavior
* Simple and easy-to-understand code structure

---

## How to Run

1. Clone the repository:

git clone [https://github.com/Ande-Lakshmi-Nishitha/google-pagerank-algorithm.git](https://github.com/Ande-Lakshmi-Nishitha/google-pagerank-algorithm.git)
cd google-pagerank-algorithm

2. Run the program:

python main.py

3. Provide input graph (if required) and view computed PageRank values.

---

## Algorithm Explanation

PR(A) = (1 - d) + d * Σ ( PR(Ti) / C(Ti) )

Where:

* PR(A) = PageRank of page A
* d = damping factor
* Ti = pages linking to A
* C(Ti) = number of outgoing links from Ti

The algorithm runs iteratively until values converge.

---

## Example

Input graph:

A → B
A → C
B → C
C → A

Output:

PageRank(A) = 0.33
PageRank(B) = 0.18
PageRank(C) = 0.49

---

## Applications

* Search engine ranking
* Social network analysis
* Recommendation systems
* Citation ranking in research papers

---

## 🛠️ Technologies Used

* Python
* Graph algorithms
* Iterative computation

---

## Future Improvements

* Visualization of graph and ranks
* Support for large datasets
* Parallel computation
* GUI interface
