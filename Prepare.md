# Prepare

In the prepare phase, [FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit) is used to explores daily usage of the smart device by its users.

## Data storage

In this case study, the tracker data were downloaded and saved in the repository. The data is stored in a long format where csv files expands vertically.

## Dataset License

The dataset is under license CC0: Public Domain, which means one can copy, modify, distribute and perform the work, even for commercial purposes, all without asking permission. It allow us to copy, perform data analysis for marketing analysis for Bellabeat on this dataset.

## Feature and Limitations of the dataset

The data is original as the dataset is directly generated from the survey distributed to Amazon mechanical turk. Also, the dataset cover the detailed tracker data from a non Bellabeat product, which can provide important information for us to finding the answer to the business task. However, there is some limitations on the dataset:

1. The data may not be highly reliable as the sample size has only 30 fit-bit users within a single website (Amazon mechanical turk), there may be a sampling bias present in the dataset.
2. The data has only the fitbit data dated back from 4/11/2016 to 05/12/2016, which may not show the latest trend trends in smart device usage.
3. The data is gathered from Amazon mechanical turk, which may not give the most reliable data source.

## Dataset overview

In this dataset, we have two folders storing the data recorded by Fitbit tracking device in two date range (04/11/2016 to 03/12/2016 and 04/12/2016 to 05/12/2016). The folder include csv file listed below:

- dailyActivity: A daily record of distance travelled, calories burned and time duration of the activity from the user, categorised by intensity.
- heartrate_seconds: Heart rate measured very 5 seconds.
- hourlyCalories: Hourly calories burned.
- hourlyIntensities: Hourly intensity of the user.
- hourlySteps: Steps took by the user every hour.
- minuteCaloriesNarrow: Calories burned every minute.
- minuteIntensitiesNarrow: Intensity measured every minute.
- minuteMETsNarrow: Metabolic equivalent of task every minute, could be used to determine intensity of a task.
- minuteSleep: logging the state of sleep every minute when the user sleeping.
- minuteStepsNarrow: Steps took by the user every minutes.
- weightLogInfo: Weight related information logged into the device.
