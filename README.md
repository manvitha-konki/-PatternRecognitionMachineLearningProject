# PatternRecognitionMachineLearningProject
Predicting BMI and gender from facial features using computational models and Leveraging deep learning for accurate predictions using ResNet50.
# Overview
## Objective: 
Predict BMI and classify gender using facial images while addressing challenges like variations in age, ethnicity, and lighting conditions.
## Dataset: 
Includes front and side facial images along with metadata (e.g., height, weight, and gender).
# BMI Categorization
The BMI is categorized into three grades based on the value:
- Underweight: BMI < 18.5
- Normal: 18.5 ≤ BMI < 25
- Overweight: BMI ≥ 25
# Model Architecture
## BMI Prediction Model:
- Utilized dual ResNet50 extractors for frontal and side view images.
- Combined features from both perspectives using concatenation.
- Dense and Dropout layers used to refine feature representation.
- Final layer predicts BMI as a continuous value with linear activation.
- Architecture enhances prediction accuracy by leveraging complementary views.
- Layers: Dense (64), Dropout (0.3), Output (1 neuron, linear activation for BMI prediction).
## Gender Classification Model:
- Single ResNet50 feature extractor used for frontal images.
- Dense layers process extracted features for classification.
- Output layer with sigmoid activation for binary classification (Male/Female).
- Binary Cross-Entropy used as the loss function.
- Optimized with Adam and evaluated using Accuracy metric.
- Layers: Dense (64), Dropout (0.3), Output (1 neuron, softmax for gender categories).
# Results
## BMI Prediction:
- MAE: 3.48, MSE: 20.29, R²: 0.21, Pearson Correlation: 0.46
- Accuracy in categorization: 75.95%
## Gender Classification:
- Accuracy: 97.66%

