MLflow Experimentation 

used link: https://mlflow.org/docs/latest/tutorials-and-examples/tutorial.html

Working flow:
Step 1 : Create virtual Env and install mlflow 
Step 2 : read csv file( Here i have done experimentation on Winequality dataset)
(https://github.com/shivashankar066/Mlflow_model_Experiments/blob/main/winequality-red.csv)
Step 3: run with python app.py and tou can give your own hyperparametrs as alpha and l1_ratio
 For Ex: python app.py 0.3 0.5
Step 4: Check its experiments in mlflow UI using cmd mlflow ui
Step 5: Continue and track with this experiments.

### Use Dagshub remote server for tracking the Experiments
Below is the details:

MLFLOW_TRACKING_URI=https://dagshub.com/shivashankar066/Mlflow_model_Experiments.mlflow \
MLFLOW_TRACKING_USERNAME=shivashankar066 \
MLFLOW_TRACKING_PASSWORD=1744652595b4c0e05cf14bcdde51be4e43e8fcba \
python script.py

# Now Export all above details from git bash
For Ex: 
open git bash in your project folder direcory  or in pycharm and then use as 
export MLFLOW_TRACKING_URI=https://dagshub.com/shivashankar066/Mlflow_model_Experiments.mlflow
export MLFLOW_TRACKING_USERNAME=shivashankar066
export MLFLOW_TRACKING_PASSWORD=1744652595b4c0e05cf14bcdde51be4e43e8fcba
and finally Run in bash command as python app.py so that all tracking experiments will appear in DagsHub

Below are the DagsHub links for Experimentations of metrics: 
Ref: https://dagshub.com/shivashankar066/Mlflow_model_Experiments/experiments/#/
Ref: https://dagshub.com/shivashankar066/Mlflow_model_Experiments.mlflow/#/experiments/0?searchFilter=&orderByKey=attributes.start_time&orderByAsc=false&startTime=ALL&lifecycleFilter=Active&modelVersionFilter=All%20Runs&selectedColumns=attributes.%60Source%60,attributes.%60Models%60&isComparingRuns=false&compareRunCharts=dW5kZWZpbmVk