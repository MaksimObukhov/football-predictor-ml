# Football match outcome prediction

## Project Overview

Football is a globally popular sport, and millions of people engage in predicting match outcomes. This project aims to leverage machine learning to predict the outcomes of football matches using a dataset spanning 22 seasons across 21 top European football leagues from 11 countries. The project involves two main tasks: a classification task predicting match outcomes (Home Win, Draw, Away Win), and a regression task predicting the number of goals scored in a match.

## Dataset Information

### Structure
- **Train Data:** Seasons from 2000/01 to 2021/22.
- **Test Data:** Season 2022/23.

### File Structure
- Data files are stored in the path (train/test)/{country}/{league}/{season}.csv.
- League is a number (lower number indicates a higher league).
- Season is in the format {start_year}{end_year}.

### Data Description
- Refer to the file `notes.txt` in the `data_description` folder for column meanings and an example in `example.csv`.

## Assignment Tasks

### Task 1: Dataset Preparation
- **Objective:** Prepare data for training using any model.
- **Steps:**
  - Handle missing values, outliers, and inconsistencies.
  - Use external data if necessary.
  - Create new features.
- **Submission:** Well-documented code explaining preprocessing decisions.

### Task 2: Classification
- **Objective:** Train a model predicting match outcomes (Home Win, Draw, Away Win).
- **Steps:**
  - Train the model on Task 1 data.
  - Explain model decisions.
  - Evaluate model performance across countries and leagues.
- **Bonus Task:** Create a betting strategy based on the model.

### Task 3: Regression
- **Objective:** Train a model predicting the number of goals scored in a match.
- **Steps:**
  - Train the model on Task 1 data.
  - Explain model decisions.
  - Evaluate model performance across countries and leagues.
- **Bonus Task:** Create a betting strategy based on the goal prediction model.

## Evaluation and Grading
Solution is evaluated based on the performance of the model on the test data. Tasks 2 and 3 will be evaluated separately. The performance of the model will be compared to the performance of other teams using the following scheme:

* score within the interval (PT − (PT − PM) · 0.25, PT] – 12.5 points.  
* score within the interval (PT − (PT − PM) · 0.5, PT − (PT − PM) · 0.25] – 10 points.  
* score within the interval (PM, PT − (PT − PM) · 0.5] – 7.5 points.  
* score within the interval (PM − (PT − PM) · 0.25, PM] – 5 points.  
* score within the interval (PM − (PT − PM) · 0.5, PM − (PT − PM) · 0.25] – 2.5 points.  

Here,  
PT is the performance of the best team, PM is the median performance of all teams.  

The maximum number of points that a team can obtain is 25, with 12.5 for Task 2 and 12.5 for Task 3.  
The performance of a team is the F-score for the classification task and MAE for the regression task. The scheme is designed to reward teams that perform better than the median. Only teams with very bad performance will end up without any points...
