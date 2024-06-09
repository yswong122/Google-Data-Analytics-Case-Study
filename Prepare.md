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

- dailyActivity: A daily record of distance travelled, calories burned, step took and time duration of the activity from the user, categorised by intensity.
- dailyCalories: A daily record of calories burned from the user. (Csv file presents only in 04/12/2016 to 05/12/2016)
- dailyIntensities: A daily record of time duration of the activity from the user, categorised by intensity. (Csv file presents only in 04/12/2016 to 05/12/2016)
- dailySteps: A daily record of step tookfrom the user. (Csv file presents only in 04/12/2016 to 05/12/2016)
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
- minuteCaloriesWide: Wide format of calories burned every minute. (Csv file presents only in 04/12/2016 to 05/12/2016)
- minuteIntensitiesWide: Wide format of intensity measured every minute. (Csv file presents only in 04/12/2016 to 05/12/2016)
- minuteStepsWide: Wide format of step took by the user every minute. (Csv file presents only in 04/12/2016 to 05/12/2016)
- sleepDay: Summarised daily sleeping time for each user. (Csv file presents only in 04/12/2016 to 05/12/2016)

### Wide csv vs Narrow csv

As minuteCalorieWide, minuteIntensitiesWide and minuteStepsWise is the wide format of the narrow equivelent csv files. The three dataset will not be analysed as narrow format would be more suitable for this case study and there is no equivelent dataset in date range from 04/11/2016 to 03/12/2016.

### Csv presented in only one of the date range

dailyCalories, dailyIntensities, dailySteps and sleepDay only present in one of the date range and some of the information has already included in dailyActivity in both date range, so in this case study, the three csv will not be considered.

### Hourly tracking data vs tracking data in minute

As hourlyCalories, hourlyIntensities and hourlySteps are just a summarised version of minuteCaloriesNarrow, minuteIntensitiesNarrow and minuteStepsNarrow, the lower grain csv equivelents (minuteCaloriesNarrow, minuteIntensitiesNarrow, minuteStepsNarrow) will be used in the next steps.

### Conclusion

At the end, the following csv file are processed and analysed in the following steps:

- dailyActivity
- heartrate_seconds
- minuteCaloriesNarrow
- minuteIntensitiesWide
- minuteMETsNarrow
- minuteSleep
- minuteStepsNarrow
- weightLogInfo
