**Predicting Income levels Using Supervised Machine Learning Algorithms: A Study on the United States Census 1994 Dataset**

This project aims to predict the income level of individuals using socio-economic features from the United States Census 1994 dataset: by employing several Supervised Machine Learning (ML) algorithms. The main objective of this study is to classify people’s income into two levels, below or equal to $50k or higher than $50k in a year. This study incorporates machine learning model selection, data preprocessing, and exploration, followed by model deployment and evaluation, and a comparative analysis of the model’s performance. The study indicates a major bias in income distribution, gender inequality in terms of income, and other significant insights. The highest performance is offered by the XGBoost model, which has the highest evaluation metrics among all models used in the study; other models like Random Forest and Gradient Boosting are highly accurate, with slight differences from XGBoost. However, the Decision Tree, Neural Network, and Support Vector machine showed lower performance which might be affected by various reasons such as class imbalances. 


Overall, 8 classification ML models are used in the study and based on various comprehensive evaluation metrics like accuracy, precision, cross-validation score, confusion matrix, and more, the models are divided into high-performance and low-performance category. Each category is writen in separate jupyter notebook that you find in the Niloofar_FinalProject repository:

**HighPerformance_Models.ipynb**
1. Logistic Regression: is used for binary classification problems which provides the probability of belonging to a certain class through maximum likelihood estimation.
2. Random Forest: enhance the prediction accuracy by leveraging the results of several decision trees (mode or mean of the trees).
3. Gradient Boosting: makes a sequence of models in a way that the new model corrects the errors of the previous model until the loss function is optimized. 
4. K-Nearest Neighbor (K-NN): it assigns the class of an input based on the majority label of k-nearest neighbors within feature space, used for classification and regression.
5. XGBoost: Gradient Boosting is optimized for higher accuracy and efficiency by sequentially making decision trees.


**LowPerformance_Models.ipynb**
6. Decision Tree: is used for classification and regression by splitting the data into subsets based on certain conditions of features’ values until a homogenous subset is achieved. 
7. Neural Network (Deep Learning): is made of neurons and multiple layers, connected to capture complex patterns of data. 
8. Support Vector Machine (SVM): it makes hyperplanes in high-dimensional space to maximize the margin between classes until the best separation between classes is achieved, both for classification and regression.

**Installation Instructions** 
In terminal Type: 
1. Clone the repository: git clone https://github.com/Niloofark/Niloofar_FinalProject.git
2. Navigate the project: cd Niloofar_FinalProject
3. install the required Libraries : numpy, pandas, scikit-learn, matplotlib, seaborn, XGBoost, and Tensorflow/keras 
4. Run the project: jupyter notebook HighPerformance_Models.ipynb

**Data**
Source: The dataset is sourced from the UC Irvine Machine Learning Repository and Kaggle, containing 48,842 instances of data with 15 features related to demographic and socio-economic information.
Features: Includes age, work class, education, marital status, occupation, relationship, race, gender, capital gain, capital loss, hours per week, and native country, among others.
Preprocessing: Handled missing values by replacing them with 'Unknown', removed duplicates, and standardized continuous features. Capital gain and loss were dropped due to skewness and low correlation with income.

**Evaluation**
Metrics: Used a combination of quantitative metrics (accuracy, precision, recall, F1-score, ROC-AUC, cross-validation score, and confusion matrix) and qualitative metrics (model interpretability, robustness, feature importance, error analysis).
Results: XGBoost showed the highest performance across most metrics, followed by Logistic Regression and Gradient Boosting.

**Results**
Summary: XGBoost had the best overall performance, balancing accuracy and training time. Logistic Regression was the most interpretable, while Gradient Boosting also performed well.
Insights: The study revealed biases in income distribution, particularly gender inequality, and identified significant socio-economic factors affecting income levels.


Contributions are welcome. Please submit pull requests or issues with clear descriptions. Ensure your contributions align with the project's goals and standards.
Please contact me: karimi.ni@northeastern.edu
