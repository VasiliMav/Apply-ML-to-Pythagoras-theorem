### Apply-ML-to-Pythagoras-theorem

## MRAC01(24/25): Software III - Machine Learning for Robotic Fabrication

# DESCRIPTION:

This project explores the application of machine learning to predict the hypotenuse of right-angled triangles. Based on the well-known Pythagorean Theorem, where the hypotenuse \( c \) is computed as:
[ c = \sqrt{a^2 + b^2} \]

# OBJECTIVES: 

STEP 1: SYNTHETIC DATA GENERATION 
Generate a dataset of right-angled triangles with random lengths.

STEP 2. USE THE PYTHAGOREAN THEOREM
Compute, apply the mathematical equation of the Pythagorean theorem on the hypotenuse for each triangle.

STEP 2: MODEL TRAINING
Train  a regression model ( Linear Regression) to predict the hypotenuse.

STEP 3: MODEL EVALUATION
Evaluate the model’s predictions against true computed values.

STEP 4: VISUALIZATION
Predict and visualize hypotenuse values based on new user inputs.

STEP 5: USER INPUT AND NEW PREDICTIONS
Give the option to the user to add input for new predictions.

# DATASET DESCRIPTION:

- Size: a variety of samples ( 100-100.000) of synthetic right-angled triangles
- Parameters :
  - `A`: First length (float, range: 1–100)
  - `B`: Second length (float, range: 1–100)
  - `C`: Hypotenuse calculated using Pythagorean Theorem
- The dataset is generated programmatically and saved as a CSV file.

---

# MODEL DETAILS:

- Model Type: Linear Regression
- Input : A, B (lengths of triangle)
- Target Variable: C (hypotenuse)

- Libraries Used: `pandas`, `numpy`, `scikit-learn`, `matplotlib`

- Training Strategy: 80% training, 20% testing (`train_test_split`)
- Inference: Accepts new user input to predict hypotenuse after training.

---

# EVALUATION METRICS:

The model is evaluated on the test set using the following metrics:

- Mean Squared Error (MSE):  
  Quantifies the average squared difference between actual and predicted values.
- R² Score (Coefficient of Determination):  
  Measures how well the model explains the variability of the target variable.

Graphical output includes:

- Scatter plot of true vs predicted hypotenuse values.

# INFERENCE:

Inference refers to the prediction phase using the model on new data.
Once trained, the model can be used to predict the hypotenuse for any new right-angled triangle using the same formula learned during training.

# RUN THE PROJECT:

To run the project locally:

```bash

# CLONE THE REPOSITORY:
git clone https://github.com/VasiliMav/Apply-ML-to-Pythagoras-theorem
cd pythagoras-ml

# INSTALL DEPENDENCIES: 
pip install -r requirements.txt
See the used libraries in the Model Details.

# RUN THE MODEL TRAINING & INFERENCE:
python src/apply_ml_to_pythagoras_theorem


AUTHORS
Vasileios Mavromitros


ACKNOWLEDGEMENTS 


Marita Georganta - Robotic Sensing Expert
Huanyu Li - Robotic Researcher




