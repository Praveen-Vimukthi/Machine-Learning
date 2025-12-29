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

## Why do we need Train–Test Split?

If you test the model using the same data it learned from, it may:

❌ Memorize answers

❌ Look very accurate

❌ Fail on new (real) data

So we split the data to answer this question:

> “Can the model predict correctly on data it has never seen before?”
