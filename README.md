# PopUpSort
With the help of ChatGPT-3.5, I was able to create this sorting visualizer. 

The PopUpSort package is a Python package that visualizes the sorting algorithms: bubble sort, selection sort, and insertion sort. The package uses the Tkinter library for the graphical user interface.

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
```

### Algorithms

Replace 'algorithm' argument with any of these options:
- 'Bubble Sort' or 'b'
- 'Selection Sort' or 's'
- 'Insertion Sort' or 'i'

### Examples
```python
arr = [60,24,21,65,93,56,35,10,55,49,86,76] # Define an array
pus.sort(arr, 'b', 0.02)                    # Visualize the bubble sort of this array with a speed of 0.02s

pus.sort_rand(50, 1, 100, 'i') # Generate an array of size 50 with elements ranging from 1 to 100 and sort it using insertion sort, speed is 0.01 by default
```

# Issues
- If you close the window while the array is still being sorted, then this error will appear
```python
_tkinter.TclError: invalid command name ".!canvas"
```
- ~~The numbers can sometimes collide with other numbers, this happens when you have a big array size~~ (Fixed!)

I'm open to solutions. If you can fix it, then go ahead!
