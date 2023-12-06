# Neural-Networks-Classification
This project focuses on the analysis and classification of a unique dataset containing detailed statistics about the world's billionaires.
dataset: https://www.kaggle.com/datasets/nelgiriyewithana/billionaires-statistics-dataset

# Project Description
The goal of this project is to apply machine learning techniques, particularly neural networks, to classify billionaires into various categories. This classification is not just based on their wealth, but also on the industry sectors they dominate and whether their fortunes are self-made or inherited. Such an analysis can provide insightful trends and patterns among the world's wealthiest individuals.

# Classifications
Wealth Category Classification: This involves categorizing billionaires into different wealth brackets. It's a nuanced look at how wealth is distributed among the top echelons of society.
Industry Classification: This classification sorts billionaires based on the primary industries of their businesses, offering insights into which sectors are the most lucrative or have the most billionaires.
Self-Made vs. Inherited Wealth: This aspect of the project looks at the origins of wealth, distinguishing between self-made billionaires and those who inherited their fortunes.
Technical Overview
The project is structured as follows:

# Dataset Preprocessing: 
The initial step involves preparing the dataset for analysis. This includes cleaning the data, handling missing values, and encoding categorical variables for machine learning models.
Baseline Classifier Implementation: Before diving into neural networks, the project implements Nearest Neighbor Classifiers as a baseline for comparison.
# Neural Network Model Implementation: 
The core of the project is the development and iterative refinement of neural network models. These models are tuned for optimal performance in the multi-class classification tasks.
Evaluation and Comparison: The project concludes with a thorough evaluation of the models' performance, comparing the results of the neural network models with the baseline classifiers.
# Technologies
Python: The primary programming language used for the project.
TensorFlow and Keras: For building and training neural network models.
Scikit-learn: Used for preprocessing data and implementing baseline classifiers.
Pandas and NumPy: For data manipulation and numerical computations.
Matplotlib: For visualizing data and results.

# Results
## Nearest Neighbor Classifier (NNC):

Wealth Classification: Achieved an accuracy of 76.04%. This model had a fair performance but struggled with some imbalances in the dataset, as indicated by the confusion matrix.
Self-Made vs. Inherited Wealth: Reached a higher accuracy of 83.33%. The model was more effective in this classification, possibly due to more distinct features distinguishing these categories.
## Nearest Neighbor Classifier (NNC):

Wealth Classification: Demonstrated a lower accuracy of 39.58%. This indicates that the centroid-based approach was less effective for this dataset, likely due to overlapping feature spaces among classes.
Self-Made vs. Inherited Wealth: Improved accuracy to 67.71%, but still less effective compared to the NNC, suggesting that centroid-based classification is less suited for this data.
## Neural Network (NN) Models:

Wealth Classification: Varied accuracies (41.67% to 75.00%) across different attempts. The fluctuating performance might be due to overfitting or the complexity of the dataset. The highest accuracy (75.00%) indicates potential with further tuning.
Self-Made vs. Inherited Wealth: More consistent performance, with accuracies ranging from 65.62% to 82.29%. This shows that NN models are relatively more effective for this classification task, with the highest accuracy models likely capturing the underlying patterns well.
- Specifically, the Neural Network (NN) models were uniquely tailored to account for the imbalance within the dataset (with Class weights), a crucial step that was not mirrored in the other models used (such as the Nearest Neighbor Classifier and Nearest Class Centroid Classifier).
