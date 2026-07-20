# Interpolation-search-
# Interpolation Search in Python

## Overview

This project implements the **Interpolation Search** algorithm in Python. Interpolation Search is an efficient searching algorithm for **sorted and uniformly distributed arrays**. Instead of always checking the middle element like Binary Search, it estimates the position of the target value based on its value.

## Features

* Fast search on sorted arrays with uniform distribution
* Simple and easy-to-understand Python implementation
* Returns the index of the searched element
* Handles cases where the element is not present

## Algorithm

Interpolation Search estimates the probable position of the target using the formula:

```text
pos = low + ((target - arr[low]) * (high - low)) // (arr[high] - arr[low])
```

If the estimated position contains the target, the search is complete. Otherwise, the algorithm continues searching in the appropriate half of the array.

## Time Complexity

| Case         | Complexity   |
| ------------ | ------------ |
| Best Case    | O(1)         |
| Average Case | O(log log n) |
| Worst Case   | O(n)         |

## Space Complexity

* **O(1)** (Constant extra space)

## Requirements

* Python 3.x

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/Interpolation-search.git
```

2. Navigate to the project folder:

```bash
cd Interpolation-search
```

3. Run the program:

```bash
python Interpolation.py
```

## Example

**Input**

```text
Array: [10, 20, 30, 40, 50, 60, 70]
Target: 50
```

**Output**

```text
Element found at index 4
```

## Applications

* Searching in large sorted datasets
* Database indexing
* Information retrieval systems
* Data analysis applications

## Author

**Magesh Anand U**
