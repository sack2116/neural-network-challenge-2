# Employee Attrition and Department Prediction Model

This project builds a multi-output neural network to predict employee attrition and department using TensorFlow and Keras.

## Project Overview
The dataset includes employee attributes such as age, job involvement, and environment satisfaction, along with targets for department and attrition. The model predicts:
- **Attrition**: Whether an employee is likely to leave the organization.
- **Department**: The department to which an employee belongs.

## Features
- Multi-output neural network with shared and branch-specific layers.
- Preprocessing steps include scaling numerical data and one-hot encoding categorical features.
- Evaluation metrics include accuracy for both outputs.

## Data Preprocessing
- Categorical features (`BusinessTravel`, `Attrition`, `Department`) were encoded using `OneHotEncoder`.
- Numerical features were standardized using `StandardScaler`.

## Model Architecture
- Shared layers process the input data.
- Two branches:
  - **Attrition Branch**: Predicts attrition using binary cross-entropy.
  - **Department Branch**: Predicts department using categorical cross-entropy.

## Challenges
- Encountered an error due to shape mismatches in target and output layers.
- Attempts to resolve the issue by verifying shapes and one-hot encoding outputs were unsuccessful.

## How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
2. Install Dependencies and Run the Notebook
```bash
# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook attrition_f.ipynb

## Future Improvements
Debug and fix the shape mismatch issue in the model fitting process.
Implement additional preprocessing and feature engineering steps for better predictions.


### Acknowledgments
This project was developed as part of a coursework assignment.

Note: Due to unresolved issues with the model training, the implementation is incomplete.
