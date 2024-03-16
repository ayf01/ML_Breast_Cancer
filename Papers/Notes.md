# Sources:
- Save and Load Model: https://www.youtube.com/watch?v=br5Y-8CS26E
- ChatGPT: 
    - Question: What are the best models to use for our problem
    - Answer:
        For breast cancer classification and biomarker identification using clinical and genomic data, several machine learning models can be effective. Here are some of the best models to consider:

        1. **Logistic Regression**: This is a good starting point for binary classification tasks like predicting the type of cancer (e.g., malignant or benign).

        2. **Random Forest**: Random Forest is effective for handling high-dimensional data and capturing complex interactions between features.

        3. **Support Vector Machines (SVM)**: SVM can handle non-linear relationships between features and is particularly useful when dealing with small to medium-sized datasets.

        4. **Gradient Boosting Machines (GBM)**: GBM models, such as XGBoost or LightGBM, are powerful ensemble methods that often perform well on structured data like clinical and genomic data.

        5. **Deep Learning Models**: Deep learning models like Convolutional Neural Networks (CNNs) or Recurrent Neural Networks (RNNs) can also be explored, especially when dealing with genomic data that may have sequential patterns.

        6. **Ensemble Methods**: Combining multiple models using ensemble techniques like bagging or boosting can further improve predictive performance.

        7. **Feature Selection Techniques**: Utilize feature selection methods such as Recursive Feature Elimination (RFE) or feature importance from tree-based models to identify potential biomarkers.

        8. **Dimensionality Reduction Techniques**: Techniques like Principal Component Analysis (PCA) or t-Distributed Stochastic Neighbor Embedding (t-SNE) can help visualize and reduce the dimensionality of genomic data while preserving important information.

        It's important to preprocess the data appropriately, handle missing values, normalize or scale features as needed, and perform cross-validation to evaluate model performance effectively. Additionally, domain knowledge and feature engineering can play a crucial role in improving model accuracy and identifying relevant biomarkers.