# Notebook 
As the title of the folder shown, we would be checking the datasets for `outliers` and dropping the extreme cases. 

In this folder, we have 3 files namely:
1. `Outliers_analysis`: In this file, the first step was to check for outliers in the dataset. The `weights` and `heights` columns were examined, and any values falling below `2.5%` or above `97.5%` of the given range were removed. This was accomplished using the pandas `drop` method, which removes any rows meeting the specified condition. Additionally, it was noted that in some cases, the `diastolic` blood pressure can be higher than the `systolic` blood pressure, which is considered `incorrect` medically. Therefore, the `diastolic` and `systolic` pressure columns were examined, and any values outside of the `2.5%` to `97.5%` range were removed. After removing the outliers, the dataset was left with `60,144 rows` and `13 columns`. This step is crucial to ensure that the data is clean and reliable for further analysis.

2. `K-Modes_Clustering`: In this file, I utilized a cleaned dataset, which had been rid of any pesky outliers. After loading the data into the notebook, we proceeded to transform the dataset in a number of ways: Firstly, we transformed the `AGE` column (measured in days) into `Age_Bin`, with a 5-year quinquennial span. Secondly, we transformed the `BMI` column into Body Mass Index Classes, where each value was assigned a corresponding `BMI_Class` from 1 to 6. Finally, we calculated the `Mean Arterial Pressure (MAP)` using the `diastolic` and `systolic` columns. Once we had transformed the dataset to our satisfaction, we proceeded to drop certain columns, retaining only the `categorical` columns. We then performed `K-Modes clustering`, employing the `Elbow` method to determine the optimal `k` value. We used `Huang initialization` to build our clusters, which were then inserted back into the dataset. Next, we split our dataset into train, validation, and test subsets, building our model and assessing its performance using a variety of performance metrics focusing more on the F1-Score.




