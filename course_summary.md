# Course Summary

Note that the course summary will be updated throughout the course.


# Block 1

## Getting started

### Goals

1) navigate in the shell application: cmd or terminal
2) have python and anaconda installed, all required packages installed
3) now how to open and close, Python console, IPython console, jupyter notebook

### Content

Shell: learn shell commands like `ls, cd, pwd, mkdir, cp, mv, rm, rm -r, touch, echo, cat`
Python: download and installing anaconda, open python console, close it, install packages using anaconda
IPython: open console, getting help, advantage compared to python console
Jupyter notebook: open it, create a notebook, write code in cells, write markdown in cells, execute and create cells, delete cells, restart the kernel, close the notebook, stop the notebook server

### Resources

- https://www.datacamp.com/courses/introduction-to-shell-for-data-science
- https://www.python.org/about/
- https://ipython.readthedocs.io/en/stable/
- https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook
- https://jupyter-notebook.readthedocs.io/en/stable/
- https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
- [Howto install WSL on windows 10](https://docs.microsoft.com/de-de/windows/wsl/install-win10)
- [Howto install Anaconda into WSL](https://towardsdatascience.com/setting-up-a-data-science-environment-using-windows-subsystem-for-linux-wsl-c4b390803dd) Note: if you simply copy paste file and directory names from the blog post, you may encounter errors (e.g., because – is not the same as -). Better type the first letters of a path/filename yourself and use `Tab` to autocomplete. Note 2: In the step where it's about actually installing Anaconda, use `bash Anaconda3-2019.03-Linux-x86_64.sh`. Note 3: You may find it convenient to set up a symbolic link to your windows home directory: `ln -s /mnt/c/Users/your_username ~/windows`


### Exercises

- https://www.practicepython.org/exercise/2014/01/29/01-character-input.html
- https://www.datacamp.com/courses/introduction-to-shell-for-data-science


## Basics of python

### Goals

1) Know different ways to write and execute python code: console, script, jupyter notebook
2) Be familiar with python variables and data types, know how to access the documentation
3) Be familiar with booleans, dictionaries, if-else statements, loops, indexing, slicing, mutability, generators, iterators

### Content

- python data types: `boolean, int float, string, list, dict, tuple`
- operators: `+, -, /, *, **, %`
- methods associated with data types, e.g., essential string methods, essential list methods.
- if-elif-else statements, conditional variable assignment, `in` operator
- list and tuple indexing, dict indexing, mutability vs. immutability,
- `while` loops, `for` loops, concept of iterator and generator, using `enumerate`,  and `zip`, combining them.
- iterating through dictionaries
- list comprehension, conditional list comprehension

### Resources

- https://github.com/cne-tum/msne-datascience-2019/blob/master/notebooks/block1/block1_session2_basic_python.ipynb
- https://github.com/cne-tum/msne-datascience-2019/blob/master/notebooks/block1/block1_session3_programming_concepts.ipynb
- https://www.datacamp.com/courses/intro-to-python-for-data-science
- https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PythonForDataScience.pdf

### Exercises

- https://www.datacamp.com/courses/intro-to-python-for-data-science
- https://www.practicepython.org/exercise/2014/02/26/04-divisors.html
- https://www.practicepython.org/exercise/2014/03/19/07-list-comprehensions.html
- https://www.practicepython.org/exercise/2017/01/24/33-birthday-dictionaries.html



## NumPy

### Goals

1) What is a Numpy array, and why to use them? (motivation)
2) Importing and Generating Data
3) Getting insight about the Data (type, dimension, size, etc.)
4) Manipulating the array (arithmetic operations, transpose, etc.)
5) Slicing and Masking
6) Combining arrays
7) Saving data


### Content

- Import data:
    - `np.load()`
    - `np.loadtxt()`
    - `np.genfromtxt()`
- Creating Numpy arrays
    - `np.zeros()`
    - `np.ones()`
    - `np.random.random()`
    - `np.empty()`
    - `np.full()`
    - `np.full_like()`
    - `np.eye()`
    - `np.identity()`
- Data Inspection (assuming we have numpy a array object called `data`)
    - `data.dtype`
    - `data.ndim`
    - `data.shape`
    - `data.size`
    - `data.strides`
    - `data.min()`
    - `data.max()`
    - `data.mean()`
    - `data.std()`
    - `data.cumsum()`
- Data Transformation (assuming we have a numpy array object called `data`)
    - `data.T`
    - `data.reshape()`
    - `data.resize()`
    - `np.expand_dims()`
    - `np.ravel()`
    - `np.add()`, `np.subtract()`, `np.multiply()`, `np.divide()`, `np.remainder()`
    - `np.exp()`, `np.log()`
    - Masking using list (or array) of True and False values
- Combining multiple arrays ans splitting an array
    - `np.concatenate()`
    - `np.append()`
    - `np.hstack()`
    - `np.vstack()`
    - `np.hsplit()`
    - `np.vsplit()`
- Saving numpy arrays
    - `save()`: saves data in .npy format
    - `savez()`: Save several arrays into an uncompressed .npz archive
    - `savez_compressed()`
    - `savetxt()`

### Resources

- https://github.com/cne-tum/msne-datascience-2019/blob/master/notebooks/block1/block1_session4_numpy.ipynb
- https://www.datacamp.com/community/tutorials/python-numpy-tutorial
- [Cheat sheet](https://s3.amazonaws.com/assets.datacamp.com/blog_assets/Numpy_Python_Cheat_Sheet.pdf)


### Exercises

- https://github.com/cne-tum/msne-datascience-2019/blob/master/notebooks/block1/block1_session4_numpyexercises.ipynb
- Section 4 (NumPy) of the datacamp Introduction to Python course


# Block 2

## scikit learn

### Goals

1) Learn to apply different machine learning techniques to analyze data
2) Introduce basic principles like supervised/unsupervised learning, overfitting, hyperparameters, cross validation
3) Understand the scikit learn syntax and pipeline

### Content

- Basic principles of machine learning:
    - Data layout
    - Choosing an algorithm
    - Evaluation
    - Cross validation
- Supervised learning
    - Classification
    - Regression
    - Measuring performance
    - Support Vector Machines
    - Decision Trees
 - Unsupervised learning
    - Clustering (K-means)
    - Dimensionality reduction (PCA)
    - Density estimation (Gaussian Mixture Model)

### Resources

- We will closely follow this tutorial: https://github.com/jakevdp/sklearn_tutorial
- Corresponding lecture: https://www.youtube.com/watch?v=L7R4HUQ-eQ0
- https://scikit-learn.org/stable/
- https://www.datacamp.com/search?q=scikit&tab=courses

### Exercises

- https://www.datacamp.com/courses/supervised-learning-with-scikit-learn

## Pytorch

### Goals

1) What is pytorch and why is it useful
2) Build an artificial neural network step by step

### Content

- Pytorch compared to numpy
- Forward propagation
- Backpropagation
- Building a neural network in pytorch
- Activation functions
- Loss functions
- Classification with NNs
- Convolutional neural networks

### Resources

- We will follow the datacamp course: https://www.datacamp.com/courses/deep-learning-with-pytorch
- Intro lecture: https://www.youtube.com/watch?v=KoyUYUcEyT8
- https://pytorch.org/tutorials/ The pytorch tutorial site has great recources on a wide range of topics (GANs, RNN,Reinforcement learning etc....)
- https://github.com/udacity/deep-learning-v2-pytorch Exercises in notebook form covering a wide range of topics.

### Exercises

- https://github.com/udacity/deep-learning-v2-pytorch/blob/master/convolutional-neural-networks/mnist-mlp/mnist_mlp_exercise.ipynb


# Block 3

## Project work starts

### Coding Environments
 - Differences IDEs and editors
 - Give an overview what editors and IDEs they could use
    - in particular PyCharm, Jupyter Lab and Jupyter Notebook. 
    - other environments: Atom, VIM, Spyder, Python-IDLE, Emacs
 - Choosing an environment for this project and setting everything up (e.g. conda environment in PyCharm)
 
### Conda Environments
 - What is a Conda environment
 - Some background why we need them and why they are useful
 - Setting up new environment for the project
 - Fundamental conda commands
    - conda create -n myenv
    - conde env list
    - conda activate myenv
    - conda deactivate myenv
    - conda install PKGNAME==3.4.1
    - conda list --explicit > pkgs.txt
 
### Introducing and coosing porjects
- https://github.com/cne-tum/msne-datascience-2019/tree/master/projects

### Overview of coding languages
 - advantages and disadvantages of commonly used coding languages
 - differences between languages (purpose, compiled, ...)
    - in particular: Java, Python, C, C++, SQL, PHP
 
### For Loops
 - https://www.dataquest.io/blog/tutorial-advanced-for-loops-python-pandas/


### Coding Conventions
 - Python specific coding and naming conventions for clean code
 - naming of variables, classes, functions
 - design patterns: KISS, DRY
 - reusability of code
 - documentation of code
 
### Object Oriented Programming
 - classes, objects, inheritance
 - class attributes vs. instance attributes
 - python implementation of a class
 - https://realpython.com/python3-object-oriented-programming/
 - data camp tutorial on OOP
 
 
