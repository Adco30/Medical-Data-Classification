## Classification Comparison and fusion: SVM, Decision Trees, and Neural Networks

Implementation and comparison of three classification algorithms - Support Vector Machines (SVM), Decision Trees, and Neural Networks - on publicly available heart disease data. The dataset is already preprocessed and the classification was performed using scikit-learn. 

    (Donald Bren School of Information and Computer Sciences (ICS), Cleveland Clinic, Heart Disease Data, https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/). 
The primary goal was to improve classification accuracy by fine-tuning the models and employing decision fusion.

### Methodology

    Individual Model Training and Tuning: Trained and tuned SVM, Decision Tree, and Neural Network models using 5-fold cross-validation.
    Feature Selection: Applied Recursive Feature Elimination (RFE) and Principal Component Analysis (PCA) to improve model accuracy.
    Test Set Predictions: Used the best feature sets for trained and tuned models to make predictions on the test set.
    Model Fusion: Combined predictions from each model using majority voting.
    Evaluation and Comparison: Evaluated the fused predictions and compared them to individual model predictions.

### Results

    Support Vector Machines: Highest average accuracy achieved was 0.5833 with a linear kernel using the original feature set.
    
![im](https://user-images.githubusercontent.com/97653144/236654760-5deebf7b-acb9-4eef-878c-749dbb11e152.png)
    
    Neural Networks: Best accuracy achieved was 0.6333 for architectures 5, 7, 8, and 9.

![im](https://user-images.githubusercontent.com/97653144/236654839-4eb8adb1-04e0-4090-9bc7-119f39f29ae5.png)

    Decision Trees: Best accuracy achieved was 0.6222 with PCA features, max_depth of 7, min_samples_split of 10, and min_samples_leaf of 2.
    
![im](https://user-images.githubusercontent.com/97653144/236654815-08853e46-60ad-41fb-89bf-b979b2bf9d81.png)

    
    
### Conclusion

Confusion Matrix:

![im](https://user-images.githubusercontent.com/97653144/236654886-b799e3f0-7bdd-42aa-9ed3-3730104e1d92.png)

    Neural Network models provided the best classification accuracy at 0.6333 among the three algorithms tested.
    The Decision Fusion using Majority Voting method had an accuracy of 0.5222, lower than the accuracy of any individual model.
    Other selection techniques such as RFE and PCA were valuable in improving the accuracy of decision trees but did not have a big impact on the SVM and Neural Network models.

Loss Curve and Accuracy Curve:


[im](https://user-images.githubusercontent.com/97653144/236654927-84d6d3d9-944b-41a3-8224-ebca64b6b10b.png)

