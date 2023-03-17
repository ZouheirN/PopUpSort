# PopUpSort
With the help of ChatGPT-3.5, I was able to create this sorting visualizer. 

The PopUpSort package is a Python package that visualizes the sorting algorithms: bubble sort, selection sort, and insertion sort. The package uses the Tkinter library for the graphical user interface.

# Requirements
- Python 3.x
- tkinter library (included in most Python installations)

# Installation

### Method 1: Using pip
```
pip install popupsort
```
### Method 2: Download the source code, then open terminal in the downloaded folder (where setup.py is) and run
```
pip install .
```

# Usage
### First import the package
```
import popupsort as pus
```

### Syntax
```
pus.sort(array, algorithm, speed) # Sorting an already defined array

pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array and sort it
```

### Algorithms

Replace 'algorithm' argument with any of these options:
- 'Bubble Sort' or 'b'
- 'Selection Sort' or 's'
- 'Insertion Sort' or 'i'
