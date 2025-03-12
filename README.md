# K-Nearest-Neighbours
A retail company analyzes customer behaviour to improve product
recommendations. They have data on 20 customers, represented in a 2-dimensional space with
two purchasing behaviour metrics:
x₁: Average amount spent per purchase (in dollars).
x₂: Frequency of purchases per month.
Each customer belongs to one of two categories (y) regarding their likelihood of purchasing a
premium membership:
• y = 0 → Not interested (blue dots).
• y = 1 → Interested (red dots).
The company wants to use the k-nearest neighbours (k-NN) algorithm to classify new
customers based on this data stored in CustomerDataset_Q1.csv (columns: x₁, x₂, y).
a) Create a 2D scatter plot of the customer data using Python (e.g., Matplotlib):
• Plot x₁ (x-axis) vs. x₂ (y-axis).
• Use blue dots for y = 0 and red dots for y = 1.
• Label axes and include a legend.
b) Implement a function fnKNN(dataset, new_point, k) in Python (no external ML libraries
like scikit-learn) to perform k-NN classification:
• Input: dataset (list of [x₁, x₂, y] rows), new_point (list [x₁, x₂]), k (integer).
• Use Euclidean distance: √((x₁₁ - x₁₂)² + (x₂₁ - x₂₂)²).
• Output: Predicted y (0 or 1) based on majority vote of k nearest neighbors.
c) Assess the k-NN classifier’s performance with k = 1:
• Split the dataset into training and test sets: 80% (16 train, 4 test), 60% (12 train,
8 test), 50% (10 train, 10 test).
• Use a fixed random seed (e.g., 42) for reproducibility.
• Report accuracy (fraction of correct predictions) for each split and briefly
comment on trends.
d) Repeat Task C for k = 2, 3, and 4
