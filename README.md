# PopUpSort

<p align="center">
<a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FZouheirN%2FPopUpSort&count_bg=%23FFD43B&title_bg=%23306998&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
</p>

With the assistance of ChatGPT-3.5, I was able to create this sorting visualizer. 

The PopUpSort package is a Python package that visualizes multiple sorting algorithms. The package uses the Tkinter library for the graphical user interface.

# Requirements
- Python 3.x
- tkinter library (included in most Python installations)

# Installation

### Method 1: Using pip
```python
pip install popupsort
```
### Method 2: Download the source code, then open terminal in the downloaded folder (where setup.py is) and run
```python
pip install .
```

# Usage
### First import the package
```python
import popupsort as pus
```

### Syntax
```python
pus.sort(array, algorithm, speed) # Sorting an already defined array

pus.sort_rand(size, min, max, algorithm, speed) # Auto generate an array and sort it

pus.sort_compare(array, algorithms, speed) # Compare sorting algorithms

pus.sort_compare_rand(size, min, max, algorithms, speed) # Auto generate an array and compare sorting algorithms
```

### Algorithms

Replace 'algorithm' argument with any of these options:
- 'Bubble Sort' or 'b'
- 'Selection Sort' or 's'
- 'Insertion Sort' or 'i'
- 'Quick Sort' or 'q'
- 'Merge Sort' or 'm'
- 'Heap Sort' or 'h'
- 'Shell Sort' or 'sh'

For sorting comparision, replace 'algorithms' argument with a list of algorithms:
```python
algorithms = ['b', 's', 'i', 'q', 'm', 'h', 'sh'] # You can remove any algorithms you don't want to compare
```

### Examples
```python
arr = [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array
pus.sort(arr, 'b', 0.02)                    # Visualize the bubble sort of this array with a speed of 0.02s

pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by default

pus.sort_compare(arr, ['s','i']) # Compare selection and insertion algorithms

pus.sort_compare_rand(100, 1, 20, ['q','h','m']) # Generate an array and compare quick sort, heap sort, and merge sort
```
