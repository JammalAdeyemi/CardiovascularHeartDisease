# Notebook 
As the title of the folder shown, we would be checking the datasets for `outliers` and dropping the extreme cases. 

In this folder, we have 3 files namely:
1. `Outliers_analysis`: In this file, the first step was to check for outliers in the dataset. The `weights` and `heights` columns were examined, and any values falling below `2.5%` or above `97.5%` of the given range were removed. This was accomplished using the pandas `drop` method, which removes any rows meeting the specified condition. Additionally, it was noted that in some cases, the `diastolic` blood pressure can be higher than the `systolic` blood pressure, which is considered `incorrect` medically. Therefore, the `diastolic` and `systolic` pressure columns were examined, and any values outside of the `2.5%` to `97.5%` range were removed. After removing the outliers, the dataset was left with `60,144 rows` and `13 columns`. This step is crucial to ensure that the data is clean and reliable for further analysis.
2. `ML-SupervisedLearning`:
3. `K-Modes_Clustering`: 




