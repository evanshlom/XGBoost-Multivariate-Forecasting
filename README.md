# XGBoost Demo

XGBoost for supervised forecasting, with lambda regularization to prevent overfitting for some targets.

## Demonstration

There are 2 ipynb files which I created using jupyter lab:

Chronologically, the first python notebook is "Test and Pickle XGBoost". It trains and runs the model then saves the model to a pkl file.

The second notebook is "Load and BlindForecast". It loads and uses the pickled model to predict A1-J1 and A2-J2 (20 total targets) for future months June 2022 - May 2023.

## Virtual Environment

You can use xgb_env.yaml to set up the virtual environment using the command below, or you can follow the requirements in requirements.txt. 

```bash
conda env create --name xgb_demo_env -f xgb_env.yml
```

## Tuned Hyperparamaters 

Ridge regularization of lambda=4 (default was lambda=1) and other less significant tuning. See 1st python notebook for more.