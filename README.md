### Importing NumPy

- The standard import convention is:
```python
import numpy as np
```


### Creating Arrays

- Arrays can be created from Python lists or using built-in NumPy functions:
```python
np.array([1, 2, 3])
np.zeros((2,3))
np.ones(5)
np.arange(0, 10, 2)
np.linspace(0, 1, 5)
np.random.rand(2,3)
```


### Inspecting Arrays

- Useful properties and methods:
```python
arr.shape     # array dimensions
arr.size      # number of elements
arr.dtype     # data type
arr.ndim      # number of dimensions
```


### Indexing and Slicing

- Methods to access array elements:
```python
arr[0]
arr[1:3]
arr[::2]
arr2d[0,1]
arr2d[:,0]
arr[arr > 1]
```


### Reshaping Arrays

- Change array structure:
```python
arr.reshape((2,3))
arr.flatten()
arr.ravel()
```


### Array Math Operations

- Typical operations performed element-wise:
```python
arr + 1
arr * arr
np.add(arr1, arr2)
np.subtract(arr1, arr2)
np.dot(arr1, arr2)
```


### Aggregate Functions

- Summarize arrays by sum, min, max, etc:
```python
arr.sum()
arr.mean()
arr.std()
arr.min()
arr.max()
np.sum(arr, axis=0)
```


### Broadcasting

- Automatic expansion of dimensions for math:
```python
a = np.ones((3,1))
b = np.ones((1,3))
a + b
```


### Stacking and Concatenating

- Combine arrays:
```python
np.concatenate([arr1, arr2])
np.vstack([arr2d1, arr2d2])
np.hstack([arr2d1, arr2d2])
```


### Copying Arrays

- Use `copy()` to avoid reference issues:
```python
arr2 = arr.copy()
```


### Boolean and Fancy Indexing

- Filter arrays by condition or custom indices:
```python
arr[arr > 3]
arr[[0,2,4]]
```


### Linear Algebra Tools

- Matrix multiplication and operations:
```python
np.dot(a, b)
np.transpose(a)
np.linalg.inv(a)
np.linalg.eig(a)
```


### Random Module

- Generate random arrays:
```python
np.random.rand(5)
np.random.randint(1, 10, (2,3))
np.random.seed(42)
```


### Saving and Loading Arrays

- Useful for large datasets:
```python
np.save('filename.npy', arr)
np.load('filename.npy')
np.savetxt('filename.txt', arr)
np.loadtxt('filename.txt')
```


### Vectorization

- Write "for loop-free" efficient code:
```python
y = a**2 + 3*a + 4
```


### Applying Functions

- Use universal functions (ufuncs) directly:
```python
np.sin(arr)
np.exp(arr)
np.sqrt(arr)
```


### Handling NaN and Inf

- Identify and manipulate:
```python
np.isnan(arr)
np.isinf(arr)
np.nan_to_num(arr)
```


***

This repository covers the core essentials for NumPy, from basic usage to advanced techniques, facilitating both beginner and advanced numerical computing tasks[1][2][3][4].

Citations:
[1] Python Numpy Tutorial (with Jupyter and Colab) https://cs231n.github.io/python-numpy-tutorial/
[2] NumPy for Image Processing https://www.kdnuggets.com/numpy-for-image-processing
[3] NumPy Tutorial https://www.w3schools.com/python/numpy/default.asp
[4] NumPy: the absolute basics for beginners https://numpy.org/doc/stable/user/absolute_beginners.html

