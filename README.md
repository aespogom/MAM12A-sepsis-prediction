# Predicting in-hospital mortality for septic patients: an explainable machine learning approach.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)

## Introduction

Sepsis is a serious medical emergency, which treatment is hard to manage. Unfortunately, sepsis often leads to death. Different courses of treatment are possible, but it is uncertain which factors contribute to the death of these patients. This study therefore focuses on predicting in-hospital mortality, using explainable machine learning methods to uncover the underlying features which are most important in these predictions. We aim to answer the question of which features contribute the most to in-hospital mortality. We use a LSTM model to make the predictions. For post-hoc explainability we use integrated gradients and TimeShap. As intrinsically interpretable models we use logistic regression and Random Forest. 
The LSTM model has an AUC of 0.835.

## Getting Started

You will need a Google Cloud account and access to the AmsterdamUMCDB.

The database, although de-identified, still contains detailed information regarding the clinical care of patients, so must be treated with appropriate care and respect and cannot be shared without permission. To request access, go to the [Amsterdam Medical Data Science website](https://amsterdammedicaldatascience.nl/).

## Usage

For the full pipeline to work, you will need to join all notebooks into one so that:

1- the data is correctly collected and processed

2- the model is trained and tested

3- the interpretability methods are applied to the results

Be aware that the time required to get the full pipeline to work is higher than 4 hours.

## Folder Structure

The project follows a enumerated folder structure.

Here's a brief description of some important folders and files:

- `01 feature_preprocessing - categorical`: Contains the code required to extract the categorical features of interest from the septic cohort.
- `02 feature_preprocessing - numerical`: Contains the code required to extract the numerical features of interest from the septic cohort.
- `03 LSTM_model`: Contains the code required to build, train and test the LSTM model.
- `04 Interpretability`: Contains the code required to perform the post-hoc interpretability methods.
- `models_LSTM/LSTM_checkpoint_12-12-2023`: Contains the weights of the best LSTM model.

## Contributing

If you'd like to contribute to the project, you can follow these steps:

1. Fork the project repository.
2. Create a new branch for your feature or bug fix.
3. Make the necessary changes in your branch.
4. Test your changes to ensure they work as expected.
5. Commit your changes and push them to your forked repository.
6. Open a pull request in the original repository

 and provide a detailed description of your changes.