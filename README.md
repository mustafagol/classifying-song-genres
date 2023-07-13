These recommendations are so on point! How does this playlist know me so well?
![](https://github.com/mustafagol/classifying-song-genres/blob/1555e163868397d9a4b1b2dab5a706ef225871fc/Classify%20Song%20Genres%20from%20Audio%20Data/music_recom.jpeg)


# Classify Song Genres from Audio Data

This repository contains code for classifying music tracks into different genres using machine learning techniques. It utilizes the FMA (Free Music Archive) dataset, which includes track metadata and audio metrics.

# Data Preparation
The initial steps involve reading and merging the track metadata and audio metrics data. The necessary libraries and datasets are imported, and the data is prepared for further analysis.

# Exploratory Data Analysis
The code includes exploratory data analysis to gain insights into the data. It creates a correlation matrix to examine the relationships between different audio metrics. The correlation matrix is visualized using a gradient color scheme.

# Feature Scaling
Before training the models, feature scaling is performed on the data. The StandardScaler from scikit-learn is used to standardize the features.

# Principal Component Analysis (PCA)
Principal Component Analysis (PCA) is applied to reduce the dimensionality of the data. The code calculates the explained variance ratios and plots them using a barplot. Additionally, it determines the number of principal components required to explain a certain amount of variance (in this case, 85%).

# Model Training and Evaluation
Two classification models, Decision Tree and Logistic Regression, are trained and evaluated using the scaled and transformed data. The models are trained on the original imbalanced dataset, and classification reports are generated to assess their performance.

# Balancing the Dataset
To address the class imbalance issue, the code creates a balanced dataset by sampling an equal number of rock and hip-hop tracks. The models are trained and evaluated on this balanced dataset, and new classification reports are generated.

# K-Fold Cross-Validation
K-Fold Cross-Validation is applied to obtain a more robust evaluation of the models' performance. The code sets up K-Fold Cross-Validation, trains the models using the pipelines, and calculates the mean accuracy scores.

# Notes
- The code assumes that the dataset files (fma-rock-vs-hiphop.csv and echonest-metrics.json) are located in a directory named datasets within the project folder. Please ensure that you have the dataset files available in the correct location before running the code.
- The code utilizes various libraries, including pandas, scikit-learn, matplotlib, and numpy. Make sure these libraries are installed in your environment before running the code.
- This code was last updated in September 2021. Please refer to the documentation of the libraries and APIs used for any updates or changes since then.
- The classification models used in this code are basic examples and may not provide the best performance. Feel free to explore and experiment with other models and techniques to improve the classification accuracy.
