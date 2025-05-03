## ✅ What I Learned
- Differences between AI, ML, and DL
- Types of ML: Supervised, Unsupervised, Reinforcement
- ML workflow and real-world uses

## 🛠️ Tools Used
- YouTube (for learning)
- Markdown (for notes)

## ⭐ Topics
- What is Machine Learning?
- Types of Learning
- Popular ML applications

## 💻 Code Preview
```python
# Just a visual idea, no code this week
# ML Types: Supervised, Unsupervised, Reinforcement
print("AI -> Simulates human intelligence")
print("ML -> Learns from data (subset of AI)")
print("DL -> Uses neural networks (subset of ML)")

applications = ["Healthcare", "Finance", "Self-driving cars", "Robotics"]
print("Applications of ML:")
for app in applications:
    print("-", app)


---

### 🗓️ **Week 2: Python Basics for Machine Learning**

```markdown
## ✅ What I Learned
- Understanding Python basics (Variables, Loops, Functions)
- Python syntax essentials for ML

## 🛠️ Tools Used
- Python (3.10+)
- Jupyter Notebooks

## ⭐ Topics
- Data types (int, float, string)
- Conditionals and loops
- Functions and modular programming

## 💻 Code Preview
```python
def greet(name):
    return f"Hello, {name}!"

names = ["Alice", "Bob", "Charlie"]
for name in names:
    print(greet(name))


---

### 🗓️ **Week 3: NumPy & Pandas for Data Analysis**

```markdown
## ✅ What I Learned
- Working with NumPy arrays for efficient computation
- Pandas for data manipulation and analysis

## 🛠️ Tools Used
- NumPy
- Pandas

## ⭐ Topics
- NumPy arrays and basic operations
- Pandas DataFrames for tabular data

## 💻 Code Preview
```python
import numpy as np
import pandas as pd

arr = np.array([1, 2, 3, 4, 5])
print("Array mean:", np.mean(arr))

df = pd.DataFrame({
    "Name": ["Alice", "Bob", "Charlie"],
    "Score": [85, 90, 95]
})
print(df.describe())
