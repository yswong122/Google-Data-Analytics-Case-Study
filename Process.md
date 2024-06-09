# Process

## Tool used

R is used in this case study as the tool for processing the data because of the scale of the data that I need to work with,
the ability for the R markdown document to be recreated by teammate and the ability to create data visuallisation within the same program.

## Transform the data

### Rename columns

Column Names for all imported file are changed to snake case for easier reading. Date and datetime column will be rename as `date` and `datetime` for easier reading and comparison in analysis stage.

### Data types

The datatype of Date and datetime column in the imported csvs were changed from character accordingly.

Date and time column are also separated for the next step.

### Categorise columns

There are some columns that are in numeric presentation of a categorical information.

According to [Data Dictionary in fitbase](https://www.fitabase.com/media/1930/fitabasedatadictionary102320.pdf), the following column can be transformed:

- intensity (in MinuteIntensity)
- value (in MinuteSleep)

### Accurate METs

According to the data dictionary above,all MET values exported from Fitabase are multiplied by 10. Therefore, METs value in minuteMETs will be divided by 10.
