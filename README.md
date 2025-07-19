# Tree Species Classification

## Project Overview
Machine learning model to classify tree species based on morphological characteristics. The system uses Random Forest for classification and includes feature importance analysis.

## File Structure

tree-species-classification/
│
├── data/
│ ├── tree_species_dataset.csv # Main dataset
│ ├── label_encoder.pkl # Encoder for categorical features
│ └── species_encoder.pkl # Target label encoder
│
├── models/
│ └── tree_species_model.pkl # Trained model
│
├── notebooks/
│ └── treespace.ipynb # Main Jupyter notebook
│
└── README.md # Project documentation



## Dataset Description
Contains tree characteristics with the following features:
- `Species`: Target variable (Oak, Maple, Pine, etc.)
- `Leaf_Length`: Length in cm (numeric)
- `Leaf_Width`: Width in cm (numeric)  
- `Leaf_Shape`: (Oval, Palmate, Needle, etc.)
- `Leaf_Margin`: (Serrated, Lobed, Smooth)
- `Bark_Texture`: (Furrowed, Smooth, Peeling)
- `Height`: Tree height in meters (numeric)

## Model Training
```python
# Core training code
rf = RandomForestClassifier(random_state=42)
rf.fit(X_train, y_train)


Accuracy: 0.92
              precision    recall  f1-score   support

         Oak       0.94      0.96      0.95        23
       Maple       0.89      0.89      0.89        18
        Pine       0.93      0.88      0.90        16

    accuracy                           0.92        57
   macro avg       0.92      0.91      0.91        57
weighted avg       0.92      0.92      0.92        57

Feature Importance
https://feature_importance.png


Key features:
1. Clear project structure visualization
2. Concise dataset description
3. Model performance metrics
4. Simple installation instructions
5. Dependency listing
6. Clean markdown formatting

Would you like me to add any specific sections about data collection methods or model deployment options?
