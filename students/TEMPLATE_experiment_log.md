# Experiment Log (Arun Krishnan)

For each experiment you run this semester:
1. Copy the template block below.
2. Fill it in.
3. Add it to the bottom of this file.

---

## Experiment Template

### Run #: 
### Date:
### Goal / Question:
(What are you testing or curious about?)

### Setup:
(What data, model, hyperparameters, preprocessing did you use?)

### Results:
(Key metrics: accuracy, precision/recall, confusion matrix, etc.)

### Reflection:
(What worked? What didn’t? What would you try next?)

# Experiment Log (Arun Krishnan)

For each experiment you run this semester:
1. Copy the template block below.
2. Fill it in.
3. Add it to the bottom of this file.

---
## Experiment Template

### Run 1: 
### Date:
### Goal / Question:
(What are you testing or curious about?)
Hyperparameters
### Setup:
(What data, model, hyperparameters, preprocessing did you use?)
random forset n_estimators = 200, min_samples_split = 2, random_state = 42, max depth.
### Results:
(Key metrics: accuracy, precision/recall, confusion matrix, etc.)
f1 score
### Reflection:
(What worked? What didn’t? What would you try next?)

none: 0.85
10:0.86
20:0.87
not much difference between parameters
# Experiment Log (Arun Krishnan)

For each experiment you run this semester:
1. Copy the template block below.
2. Fill it in.
3. Add it to the bottom of this file.

---
## Experiment Template

### Run 2: 
### Date:
### Goal / Question:
(What are you testing or curious about?)
search methods for hyperparameters
### Setup:
(What data, model, hyperparameters, preprocessing did you use?)
Gridsearch randomizedsearch
### Results:
(Key metrics: accuracy, precision/recall, confusion matrix, etc.)
Running GridSearchCV...
Running RandomizedSearchCV...
Best params (GridSearch): {'max_depth': 20, 'n_estimators': 100}
Best score (GridSearch): 0.863
Best params (RandomizedSearch): {'max_depth': 20, 'min_samples_split': 4, 'n_estimators': 121}
Best score (RandomizedSearch): 0.864
### Reflection:
(What worked? What didn’t? What would you try next?)
- Which method finished faster? Why?  randomized search cv. it only tests randomized values of what gridsearch does, oftentimes being smaller
- Did they find similar or different best parameters?  similar but randomized search was better because it explored one extra parameter (most likely)
- When would you choose GridSearchCV vs RandomizedSearchCV in practice?  Grid search when not caring much about efficiency but wanting best results and vice versa.

# Experiment Log (Arun Krishnan)

For each experiment you run this semester:
1. Copy the template block below.
2. Fill it in.
3. Add it to the bottom of this file.
---

# Example Experiment Log — Taiwo 

## Run 1 — 2025-09-04
- **Goal / Question**: What happens if I change `n_estimators` from 100 to 200?
- **Setup**: Baseline Random Forest, train/test split = 80/20
- **Results**: Accuracy = 0.84, Precision = 0.72, Recall = 0.66
- **Reflection**: Increasing estimators gave a small accuracy bump. Took longer to train. Worth it? Maybe.

---

## Run 2 — 2025-09-06
- **Goal / Question**: Compare Random Forest vs Logistic Regression
- **Setup**: Same preprocessing as before
- **Results**: RF Acc = 0.85, LogReg Acc = 0.79
- **Reflection**: LogReg underfit the data. Nice reminder that not all models capture interactions.
