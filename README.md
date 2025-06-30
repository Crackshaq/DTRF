Task 5: Decision Trees and Random Forests 

Tools & Libraries
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Graphviz (for tree visualization)


Dataset
I used the [Heart Disease Dataset]

 How I Did This Project

1. Loaded and Explored the Dataset  
   Used `pandas` to load the CSV file and checked for missing values and data types.

2. Split Data for Training and Testing  
   I separated the features (`X`) and target (`y`), then split the data into training and testing sets using `train_test_split()`.

3. Trained a Decision Tree Classifier  
   Created a `DecisionTreeClassifier`, trained it on the training data, and predicted values on the test set.

4. Visualized the Decision Tree  
   Used `export_graphviz()` and `graphviz.Source()` to generate a clean and colorful visualization of the trained decision tree.

5. Analyzed Overfitting  
   I experimented with limiting the tree’s depth using the `max_depth` parameter to avoid overfitting and compared accuracies.

6. Trained a Random Forest Classifier  
   Trained a `RandomForestClassifier` with 100 trees, and compared its accuracy with the Decision Tree. Random Forest performed better.

7. Evaluated with Cross-Validation 
   Used `cross_val_score()` with 5-fold CV to get a more reliable performance estimate.

8. Interpreted Feature Importances  
   Extracted feature importances from the Random Forest model and plotted them using `matplotlib` to understand which features were most influential
