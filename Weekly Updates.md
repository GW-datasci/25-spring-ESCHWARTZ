## Weekly Updates

# Week 1:

- research on cross validation with time series data
- began EDA
  - exploring data indicated that each subject has two data frames so a next step will be understanding how to add the data frames together
- I am still working on figuring out how I will be organizing my data set and what the final dataset will look like, but beginning my EDA helped with this!
EDA showed that the data frames are in different time delineations, so I will also need to figure out how I will merge these data frames based on these time differences
scheduled call with Prof Majhi to discuss time data issue and topological data analysis as a different potential solution
I was thinking for the data frame that has fewer rows, I could multiply each row by 8 to stretch the data out while maintaining the distribution
multiplying each row by 8 would bring the smaller data frame to the size of the larger data frame and make each row in the formerly small data frame the equivalent of 1/8th second instead of 1 second as it is currently organized

# Week 2:

- I met with Prof Majhi regarding my data discussed in the last point above
  - We decided that I should replicate each entry and follow the plan I had above for syncing my data up. 
  - I visualized this data to ensure that the data looked correct. 
- For some of the subjects, there is more data than others, but only by +/- 400 data points. To mitigate this, I plan on using mean imputation from the prior section to aid in adding the missing values at the end for some of the subjects. 
  - To ensure I am not cutting any data out given that would indicate data loss, I will first find the subject with the most data points, then align the rest of the subjects with the same quantity of total data points.

# Week 3:

- I merged the data to create dataframes and .csv files for each subject.
- I finished planning out my data processing steps, and my next step is focused on understanding splitting time series data, as I want to ensure I am not influencing potential test data with data processing steps.
  - Understanding the time series train/test split is my focus for this upcoming week, then once the split is solidified, I will perform data processing steps in accordance with traditional machine learning data processing steps.
  - I also found this source to aid in my time series data processing steps: https://www.sciencedirect.com/science/article/pii/S2307187724000452#sec0015
- After some further research, I have determined that I don't think I will need to impute data because technically, for each data frame, there is no data missing.
  - I will have further insights into this once I finish my time series research.
