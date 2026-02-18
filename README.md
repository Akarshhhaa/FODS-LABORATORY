# T-Test Program (One Sample)

import math

# Sample data
data = [45, 50, 55, 60, 48, 52, 49, 53]

# Hypothesized mean
mu = 50

# Step 1: Calculate sample mean
mean = sum(data) / len(data)

# Step 2: Calculate standard deviation
variance = sum((x - mean) ** 2 for x in data) / (len(data) - 1)
std_dev = math.sqrt(variance)

# Step 3: Calculate T-statistic
t = (mean - mu) / (std_dev / math.sqrt(len(data)))

print("Sample Mean:", round(mean, 2))
print("Standard Deviation:", round(std_dev, 2))
print("T-Statistic:", round(t, 3))

