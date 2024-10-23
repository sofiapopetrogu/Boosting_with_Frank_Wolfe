# Boosting_with_Frank_Wolfe

### Project Overview
In this project, we analyze and implement a boosting algorithm proposed by Mitsuboshi, et al. 2022 in their paper 'Boosting as Frank-Wolfe' that seeks to maximize the soft margin of a linear combination of hypotheses from weak learners.

### Project Members
- Fairouz Baz Radwan
- Sofia Pope Trogu

### Timeline
June 2024

### Key Features
- **Algorithm Analysis and Theory**: Frank-Wolfe and Linear Programming Boosting Algorithms explained with mathematical analysis and pseudocode.
- **Algorithm and Decision Tree Classifier Definitions**: Variants of a linear program boosting algorithm with options to apply Frank-Wolfe update rules were developed, along with a custom decision tree classifier as a base learner.
- **Hyperparameter Tuning**: Ran k-fold cross validation scheme to identify best capping hyperparameter as a constraint on distribution in boosting algorithms.
- **Performance Metrics**: Performance for each algorithm on experimental data measured using test accuracy, test error, time to reach soft margin objective, computing time, and number of LPBoost weight updates chosen over FW strategy updates. 

### Datasets
The algorithms were tested and compared on two datasets: Breast Cancer and Thyroid from sklearn and Gunnar Rätsch's benchmark datasets, respectively. Key data preprocessing steps include:  
1. Assigning target labels as [-1, 1]
2. Train-test split

### Libraries Used
- `matplotlib.pyplot`: Data visualization.
- `numpy`, `pandas`, `os`, `tqdm`, `time`: Data manipulation and time handling.
- `pulp`: Linear Programming Optimizer.
- `sklearn.model_selection`: train-test split and k-fold scheme set-up.
- `sklearn.datasets`: Loading sklearn datasets

### Visualizations
The project includes several plots that report performance metrics, such as convergence to soft-margin objective, behvaior of test error over time, and the number of LPBoost updates, across the algorithm variants for each experimental dataset.
