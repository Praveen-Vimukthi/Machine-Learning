# What is Train–Test Split?

Imagine this 👇

You are studying for an exam.

- You learn from a book → this is training
- Then you take a test → this is testing

In **Machine Learning**, it is the same idea.

👉 We split the data into two parts:

- Training data → to teach the model
- Testing data → to check how well it learned

This is called Train–Test Split

--- 

## Why do we need Train–Test Split?

If you test the model using the same data it learned from, it may:

❌ Memorize answers

❌ Look very accurate

❌ Fail on new (real) data

So we split the data to answer this question:

> “Can the model predict correctly on data it has never seen before?”

---

## Simple Example

Suppose we have this dataset:

|**Hours Studied** | **Marks** |
| -------------- | ----- |
| 1             | 20    |
| 2             | 40    |
| 3             | 60    |
| 4             | 80    |
| 5             | 100   |

### Step 1: Split the data

Let’s say:
- 80% → Training
- 20% → Testing

### Training data (used to learn):

| **Hours** | **Marks** |
| ----- | ----- |
| 1     | 20    |
| 2     | 40    |
| 3     | 60    |
| 4     | 80    |

### Testing data (used to test):

| **Hours** | **Marks** |
| ----- | ----- |
| 5     | 100   |

---

## What happens during training?

The model learns this pattern:

> “If study hours increase, marks increase.”

It learns using only training data.

---

## What happens during testing?

Now we ask the model:

> “If a student studies 5 hours, what marks will they get?”

- **Actual answer:** 100
- **Model prediction:** maybe 95 or 102

If prediction is close → **good model**
If prediction is far → **bad model**

---

## Common Split Ratios

These are very common:

| **Training** | **Testing**             |
| -------- | ------------------- |
| 70%      | 30%                 |
| 80%      | 20% ✅ (most common) |
| 90%      | 10%                 |

✔ More training data = better learning

✔ Enough testing data = fair evaluation

---

## Train–Test Split in Python (scikit-learn)

```python
import pandas as pd
from sklearn.model_selection import train_test_split

# Create dataset
data = pd.DataFrame({
    'Hours_Studied': [1,2,3,4,5,6,7,8,9,10],
    'Result': ['Fail','Fail','Fail','Pass','Pass','Pass','Pass','Pass','Pass','Pass']
})

X_train, X_test, y_train, y_test = train_test_split(
    X, y,
    test_size=0.3,
    random_state=42
)

print("Train Result     Count:")
print(y_train.value_counts())

print("\nTest Result    Count:")
print(y_test.value_counts())

```
**Output:**
```
Train Result    Count:
Pass              6
Fail              1

Test Result     Count:
Pass              1
Fail              2
```
