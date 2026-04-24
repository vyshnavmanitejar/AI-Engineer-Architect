# 🔢 NumPy: Numerical Computing in Python

<div align="center">

![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![Level](https://img.shields.io/badge/Level-Beginner%20to%20Intermediate-blue?style=flat-square)
![Duration](https://img.shields.io/badge/Duration-15--20%20hours-orange?style=flat-square)
![Library](https://img.shields.io/badge/Library-NumPy%201.26%2B-red?style=flat-square)
![Topics](https://img.shields.io/badge/Topics-12%2B-purple?style=flat-square)

**Master numerical computing and array operations - the foundation of data science**

[🚀 Quick Start](#quick-start) • [📚 Learning Path](#learning-path) • [🛠️ Resources](#tools--resources) • [💡 Projects](#hands-on-projects)

</div>

---

## 📋 Table of Contents

1. [Overview](#overview)
2. [Quick Start](#quick-start)
3. [Learning Objectives](#learning-objectives)
4. [Prerequisites](#prerequisites)
5. [Learning Path](#learning-path)
6. [Tools & Resources](#tools--resources)
7. [Core Topics](#core-topics)
8. [Performance Tips](#performance-tips)
9. [Hands-On Projects](#hands-on-projects)
10. [Key Takeaways](#key-takeaways)
11. [Further Learning](#further-learning)

---

## Overview

**NumPy** (Numerical Python) is the fundamental package for numerical computing in Python. It provides powerful N-dimensional array objects and tools for scientific computing, making it essential for data science, machine learning, and scientific research. NumPy is the foundation that powers pandas, scikit-learn, TensorFlow, and virtually all data science libraries.

### Why NumPy?

| Benefit | Impact |
|---------|--------|
| **100x Faster** | C-based implementation for high performance |
| **Memory Efficient** | Compact array storage compared to Python lists |
| **Vectorization** | Eliminate loops for clean, fast code |
| **Foundation Library** | Required by pandas, scikit-learn, TensorFlow |
| **Broadcasting** | Powerful operations on arrays of different shapes |
| **Mathematical Functions** | 200+ functions for linear algebra, statistics, etc. |

---

## Quick Start

**Start Here:** [001.Introduction.ipynb](001.Introduction.ipynb)

- ⏱️ **Time Required:** 1-2 hours for basics
- 📝 **Prerequisites:** Python programming knowledge
- 🎯 **Goal:** Import NumPy and create your first array

```python
import numpy as np

# Create arrays
arr = np.array([1, 2, 3, 4, 5])
matrix = np.array([[1, 2, 3], [4, 5, 6]])

# Perform operations
print(arr * 2)  # [2 4 6 8 10]
print(matrix.sum())  # 21
```

---

## 📚 Learning Objectives

After completing this module, you will be able to:

| Objective | Level | Time |
|-----------|-------|------|
| ✅ Create and manipulate NumPy arrays | Beginner | 2 hrs |
| ✅ Understand NumPy data types and dtype | Beginner | 1.5 hrs |
| ✅ Perform element-wise and matrix operations | Intermediate | 2.5 hrs |
| ✅ Use broadcasting for efficient computations | Intermediate | 2 hrs |
| ✅ Index and slice arrays effectively | Intermediate | 2 hrs |
| ✅ Apply mathematical functions | Intermediate | 2 hrs |
| ✅ Perform linear algebra operations | Advanced | 2.5 hrs |
| ✅ Handle random numbers and distributions | Advanced | 2 hrs |
| ✅ Optimize code with vectorization | Advanced | 2 hrs |
| ✅ Integrate NumPy with other libraries | Advanced | 1 hr |

---

## 🎯 Prerequisites

### Required
- 🐍 Python 3.8+ proficiency
- 💻 Comfortable with variables and data types
- 📚 Understanding of basic data structures (lists, tuples)
- 🧮 Basic mathematical concepts (vectors, matrices)

### Recommended
- Familiarity with lists and list comprehensions
- Basic understanding of linear algebra
- Experience with Jupyter notebooks

---

## Learning Path

```
Week 1: Array Basics (4-5 hours)
  ├─ Array Creation Methods
  ├─ Data Types and dtype
  ├─ Array Attributes
  └─ Reshaping and Resizing

Week 2: Indexing & Slicing (4-5 hours)
  ├─ 1D Indexing and Slicing
  ├─ Multi-dimensional Indexing
  ├─ Boolean Indexing
  └─ Fancy Indexing

Week 3: Operations & Broadcasting (4-5 hours)
  ├─ Arithmetic Operations
  ├─ Broadcasting Mechanism
  ├─ Comparison Operations
  └─ Logical Operations

Week 4: Mathematical Functions (3-4 hours)
  ├─ Element-wise Functions
  ├─ Aggregation Functions
  ├─ Linear Algebra
  └─ Random Numbers

Week 5: Practical Applications (3-4 hours)
  ├─ Vectorization Patterns
  ├─ Performance Optimization
  ├─ Integration with Pandas
  └─ Real-world Projects
```

---

## 🛠️ Tools & Resources

### Installation
```bash
# Install NumPy via pip
pip install numpy

# Or via conda
conda install numpy

# Verify installation
python -c "import numpy; print(numpy.__version__)"
```

### Useful Resources
| Resource | Type | Purpose |
|----------|------|---------|
| **NumPy Docs** | Official | Complete reference |
| **NumPy Tutorial** | Tutorial | Step-by-step learning |
| **DataCamp** | Course | Interactive lessons |
| **Real Python** | Articles | Practical guides |
| **Stack Overflow** | Q&A | Troubleshooting |

### Complementary Tools
- **Pandas:** Data manipulation (built on NumPy)
- **Matplotlib:** Visualization (uses NumPy arrays)
- **Scikit-learn:** Machine learning (built on NumPy)
- **SciPy:** Scientific computing (extends NumPy)
- **IPython/Jupyter:** Interactive development

---

## Core Topics

### 📖 Section 1: Array Fundamentals (4-5 hours)

#### 1.1 Introduction to NumPy
- Why NumPy exists (speed, memory, convenience)
- NumPy vs. Python lists comparison
- When to use NumPy
- Installation and environment setup

#### 1.2 Creating Arrays
- **From Python data structures:**
  - `np.array()` from lists/tuples
  - `np.asarray()` for conversion
  - Specifying dtype during creation
  
- **Using creation functions:**
  - `np.zeros()` - arrays of zeros
  - `np.ones()` - arrays of ones
  - `np.full()` - arrays with specific values
  - `np.arange()` - like range() but for arrays
  - `np.linspace()` - evenly spaced values
  - `np.eye()` - identity matrix
  - `np.diag()` - diagonal matrix

#### 1.3 Understanding dtypes
- **Numeric types:** int8, int16, int32, int64, uint*, float32, float64, complex64, complex128
- **Other types:** bool, object, string_, unicode_
- **dtype operations:**
  - Checking dtype: `.dtype`
  - Converting dtype: `.astype()`
  - Upcasting and downcasting implications

#### 1.4 Array Attributes
- Shape and size
- Dimensions (ndim)
- Number of elements
- Itemsize and nbytes
- Strides and memory layout

#### 1.5 Reshaping Operations
- `reshape()` - change shape without copying
- `flatten()` and `ravel()` - convert to 1D
- `transpose()` - swap axes
- `squeeze()` and `expand_dims()` - add/remove dimensions

---

### 🔍 Section 2: Indexing & Slicing (4-5 hours)

#### 2.1 Basic Indexing
- 1D indexing (positive and negative)
- Multi-dimensional indexing
- Integer indexing behavior
- Indexing returns views vs. copies

#### 2.2 Slicing
- 1D slicing with start:stop:step
- Multi-dimensional slicing
- Ellipsis (...) notation
- Slice object and slicing functions

#### 2.3 Advanced Indexing
- **Boolean indexing:** Filtering with conditions
  - Creating boolean masks
  - Using boolean arrays for selection
  
- **Fancy indexing:** Using integer arrays
  - Multiple dimensions
  - Integer array indexing
  - Gather and scatter operations

#### 2.4 Common Indexing Patterns
- Extracting subarray
- Conditional filtering
- Masking operations
- Performance considerations

---

### ➕ Section 3: Operations & Broadcasting (4-5 hours)

#### 3.1 Element-wise Operations
- Arithmetic: +, -, *, /, //, %, **
- In-place operations (+=, -=, etc.)
- Comparison: ==, !=, <, >, <=, >=
- Logical: &, |, ~, xor

#### 3.2 Broadcasting Mechanism
- **Broadcasting rules:**
  1. Align dimensions from right
  2. Dimensions must be compatible
  3. Size 1 dimensions broadcast
  
- **Practical examples:**
  - Vector + scalar
  - Matrix + vector
  - Different shaped arrays
  - When broadcasting fails

#### 3.3 Aggregation Functions
- **Sum and Product:** sum, prod, cumsum, cumprod
- **Statistics:** mean, median, std, var, min, max
- **Quantiles:** percentile, quantile
- Axis parameter for dimension-wise operations

#### 3.4 Mathematical Functions
- **Trigonometric:** sin, cos, tan, arcsin, arccos, arctan
- **Exponential & Logarithmic:** exp, log, log10, log2
- **Rounding:** round, floor, ceil, trunc
- **Other:** abs, sign, sqrt, power

---

### 🧮 Section 4: Linear Algebra & Advanced Math (3-4 hours)

#### 4.1 Matrix Operations
- Matrix multiplication (@, np.dot)
- Matrix transpose and conjugate
- Trace and determinant
- Inverse and pseudo-inverse

#### 4.2 Linear Algebra Functions
- `np.linalg.solve()` - solve linear systems
- `np.linalg.eig()` - eigenvalues/eigenvectors
- `np.linalg.svd()` - singular value decomposition
- `np.linalg.qr()` - QR decomposition

#### 4.3 Random Numbers
- Random number generation
- Different distributions (normal, uniform, etc.)
- Setting seeds for reproducibility
- Sampling operations

#### 4.4 Fourier Transform
- Fast Fourier Transform (FFT)
- Inverse FFT
- Real FFT for real data
- Applications in signal processing

---

### 🚀 Section 5: Performance & Optimization (3-4 hours)

#### 5.1 Vectorization Strategies
- Identifying loops to eliminate
- Using NumPy functions instead of loops
- Broadcasting clever usage
- Performance comparison

#### 5.2 Memory Efficiency
- Understanding memory layout (C vs. Fortran order)
- Copy vs. view implications
- Memory profiling
- Optimizing for cache

#### 5.3 Performance Best Practices
- Avoid implicit copies
- Use appropriate dtypes
- Leverage NumPy's compiled functions
- Profiling and benchmarking

#### 5.4 Integration with Other Libraries
- NumPy to Pandas DataFrames
- NumPy arrays in scikit-learn
- Using NumPy with deep learning frameworks
- I/O operations (save/load)

---

## Performance Tips

### ⚡ Optimization Techniques
1. **Vectorize:** Replace loops with NumPy operations
2. **Preallocate:** Create output arrays before filling
3. **Use views:** Avoid unnecessary copies
4. **Choose dtype wisely:** float32 is faster than float64 when appropriate
5. **Leverage broadcasting:** Avoid creating unnecessary copies
6. **Use compiled functions:** NumPy functions are faster than Python loops
7. **Profile first:** Identify bottlenecks before optimizing

### 📊 Common Performance Mistakes
- ❌ Using Python loops instead of NumPy operations
- ❌ Creating unnecessary copies of arrays
- ❌ Using object dtype for numeric data
- ❌ Inefficient indexing patterns
- ❌ Inappropriate memory layout

---

## Hands-On Projects

### Project 1: Matrix Calculator 🧮
**Level:** Beginner | **Duration:** 3-4 hours
- Create matrices
- Perform arithmetic operations
- Calculate determinant and inverse
- Solve linear systems

### Project 2: Statistical Analysis 📊
**Level:** Intermediate | **Duration:** 5-6 hours
- Load sample data
- Calculate descriptive statistics
- Compute correlations
- Generate visualizations
- Handle missing data

### Project 3: Image Processing Basics 🖼️
**Level:** Intermediate | **Duration:** 6-8 hours
- Load images as arrays
- Apply filters (blur, edge detection)
- Rotate and resize images
- Enhance contrast and brightness

### Project 4: Monte Carlo Simulation 🎲
**Level:** Advanced | **Duration:** 8-10 hours
- Simulate π estimation
- Estimate integrals
- Financial simulations
- Visualize results

### Project 5: Machine Learning Pipeline 🤖
**Level:** Advanced | **Duration:** 10-12 hours
- Generate synthetic data
- Normalize features
- Implement simple algorithms from scratch
- Evaluate performance

---

## Key Takeaways

### 🎯 Core Principles
1. **NumPy arrays are fast** - 10-100x faster than Python lists
2. **Vectorization is key** - eliminate loops whenever possible
3. **Broadcasting is powerful** - learn to use it effectively
4. **Memory matters** - understand dtype and shape implications
5. **Integration is essential** - NumPy works with the whole ecosystem

### 💡 Best Practices
- Always vectorize loops
- Use appropriate dtypes for memory efficiency
- Leverage broadcasting instead of explicit reshaping
- Profile before optimizing
- Use NumPy functions instead of reinventing the wheel

### 🚀 Next Steps
1. Master the fundamentals (arrays and operations)
2. Practice with datasets and analysis
3. Learn Pandas for data manipulation
4. Apply to machine learning projects
5. Explore specialized libraries (SciPy, scikit-learn)

---

## Further Learning

### Recommended Resources
- **NumPy Official Guide:** numpy.org/doc
- **"From Python to NumPy" book:** Free online resource
- **DataCamp:** Interactive NumPy courses
- **Real Python:** Comprehensive tutorials
- **YouTube:** 3Blue1Brown for linear algebra intuition

### Advanced Topics
- Random sampling techniques
- Sparse arrays
- Memory-mapped arrays
- GPU acceleration (CuPy)
- Extending NumPy with C/Cython

### Integration Path
1. **NumPy Fundamentals** (This module) ✓
2. **Pandas** - DataFrames and data manipulation
3. **Matplotlib/Seaborn** - Visualization
4. **Scikit-learn** - Machine learning
5. **Specialized Libraries:** TensorFlow, PyTorch, etc.

---

<div align="center">

**Last Updated:** 2024 | **Version:** 2.0 (Professional Edition)

⭐ NumPy: Making Python fast! ⭐

</div>
- Comparison with Python lists
- Basic array concepts

### **Lesson 2: NumPy Data Types** 🏷️
Understanding data types for efficient storage
- **Integer types:** `int8`, `int16`, `int32`, `int64`
- **Floating-point types:** `float32`, `float64`
- **Complex numbers:** Complex arithmetic
- **Boolean types:** Logical operations
- **String and Unicode types:** Text handling
- **Structured arrays:** Custom data types
- Type casting and conversion

### **Lesson 3: Creating NumPy Arrays** 📐
Multiple methods to create arrays
- Creating arrays from Python lists
- Using `zeros()` and `ones()` functions
- Using `arange()` and `linspace()`
- Using `random()` for random arrays
- Using `eye()` for identity matrices
- Array indexing and slicing techniques
- Multi-dimensional array creation

---

## 🎯 Key Concepts

### Array Operations 🔄
- **Element-wise operations:** Addition, subtraction, multiplication, division
- **Broadcasting:** Performing operations on arrays of different shapes
- **Aggregation Functions:** Sum, mean, standard deviation, min/max
- **Shape manipulation:** Reshape, flatten, transpose

### Linear Algebra 📊
- Matrix multiplication and dot products
- Determinants and matrix inverses
- Eigenvalues and eigenvectors
- Solving linear equations
- Matrix decomposition

### Performance Benefits ⚡
- **Vectorization:** Avoid Python loops for faster computation
- **Memory efficiency:** Contiguous array storage
- **C backend:** Optimized computational kernels
- **Broadcasting:** Efficient multi-dimensional operations

### Advanced Operations 🔬
- Random number generation
- Statistical functions
- Fourier transforms
- Polynomial operations
- Memory efficiency compared to Python lists
- Optimized C implementations under the hood

## 💻 Practical Applications

- Data preprocessing and cleaning
- Scientific computing
- Statistical analysis
- Machine learning feature engineering
- Image and signal processing

## 📖 How to Use This Module

1. Start with the Introduction to understand NumPy's purpose
2. Learn about data types to make informed choices
3. Master array creation using different methods
4. Practice array operations through hands-on exercises

## 🔧 Prerequisites

- Python 3.7+
- Basic Python programming knowledge
- Familiarity with mathematical concepts

## 🔗 Related Modules

- Machine Learning
- Data Analysis
- Deep Learning (uses NumPy extensively)

## 📝 Tips for Success

- Practice array operations regularly
- Understand broadcasting rules to avoid errors
- Use NumPy's built-in functions for efficiency
- Leverage documentation with `help()` and `?` in Jupyter

---

**Last Updated:** 2026  
**Difficulty Level:** Beginner to Intermediate  
**Prerequisites:** Basic Python Knowledge
