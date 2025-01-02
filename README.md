# Rock Image Classification Project

## Project Overview
This project explores the classification of rocks into three types: **Igneous**, **Metamorphic**, and **Sedimentary**, using machine learning models. We analyzed the performance of three classification models:

1. **Softmax Regression**
2. **Support Vector Machine (SVM)**
3. **Random Forest**

After evaluating the models individually, we created an **ensemble model** combining the best-performing versions of each and compared its performance against the standalone models.

Additionally, we conducted a comparative analysis between our model's performance and human classification accuracy, including correlation analyses between model probabilities and average human accuracies.

---

## Dataset
- **Instances:** 480
- **Features:** 11 continuous features:
  1. Angular Fragments
  2. Rounded Fragments
  3. Straight Stripes
  4. Curved Stripes
  5. Physical Layers
  6. Veins
  7. Oily or Shimmery Texture
  8. Splotchy Texture
  9. Single Translucent Crystal
  10. Multiple Cubic Crystals
  11. Sandy Texture

- **Label:** Rock Type (1 = Igneous, 2 = Metamorphic, 3 = Sedimentary)

- **Source:** [OSF Repository](https://osf.io/cvwu9/wiki/Data%20File%20Descriptions/)

---

## Project Workflow

### 1. Data Preprocessing
- Normalized features to improve model performance.
- Split data into training and testing sets (80%-20%).

### 2. Model Implementation
- **Softmax Regression:** Optimized using gradient descent with various learning rates and regularization techniques.
- **Support Vector Machine:** Explored kernel types (linear, RBF) and regularization parameters.
- **Random Forest:** Tuned hyperparameters such as the number of estimators and maximum tree depth.

### 3. Ensemble Model
- Combined the predictions of the three models using a weighted voting mechanism.
- Adjusted weights based on individual model accuracies.

### 4. Human Classification Comparison
- Measured human accuracy on the dataset through expert evaluations.
- Analyzed the correlation between model probabilities and human performance.

### 5. Evaluation Metrics
- Accuracy
- Precision, Recall, and F1-Score
- Comparative analysis between model and human classification accuracy

---

## Results

### Validation Accuracy:
- **SVM**: 0.822
- **Softmax**: 0.8
- **Random Forest**: 0.767
- **Hard Voting Model**: 0.811
- **Soft Voting Model**: 0.778
- **Stacked Model**: 0.789

### Test Accuracy:
- **SVM**: 0.744
- **Softmax**: 0.667
- **Random Forest**: 0.7
- **Hard Voting Model**: 0.756
- **Soft Voting Model**: 0.744
- **Stacked Model**: 0.733

---

## Future Work
- Explore deep learning approaches for rock classification.
- Investigate additional features or external datasets to enhance model performance.
- Improve the ensemble method to address specific shortcomings observed during human comparisons.

---

We welcome feedback and suggestions to improve our work!
