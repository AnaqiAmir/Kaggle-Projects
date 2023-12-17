# Data Science Salaries

## Overview
The Data Science Salaries dataset on Kaggle invites participants to analyze the global data science salaries and create a model to predict these salaries. The dataset includes information such as the employees experience level, employment type, job title, and of course the salaries of these employeed as well.

### Links
* Dataset: [Data Science Salaries 2023](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023)
* This notebook on Kaggle: [Data Science Salaries 2023](https://www.kaggle.com/code/anaqiamir/data-science-salaries-2023)
* My Kaggle profile: [Anaqi Amir](https://www.kaggle.com/anaqiamir)

## File Structure
* `README.md`: Overview of the repository
* `data-science-salaries-2023.ipynb`: The python notebook that consists of all the codes that I did in this competition
* `ds_salaries.csv`: The dataset

## Results

### EDA:
* Most people are have a senior level position.
* 99% of the entries have a full-time position rather than a part-time, contractual, or freelancing position.
* There are 93 unique job titles in the dataset.
* The top 10 job titles that makes up 85.75% of the dataset are:
  * Data Engineer (1040)
  * Data Scientist (840)
  * Data Analyst (612)
  * Machine Learning Engineer (289)
  * Analytics Engineer (103)
  * Data Architect (101)
  * Research Scientist (82)
  * Data Science Manager (58)
  * Applied Scientist (58)
  * Research Engineer (37)
* Applied Scientist has the highest median salary at around 200,000 USD per annum.
* Data Analyst has the lowest median salary (amongst the top 10 job titles) at around 100,000 USD per annum.
* Most companies are medium-sized as opposed to large-sized or small-sized companies.
* 83.28% of the companies in the dataset comes are based either in the US or Canada.
* Including the companies that are based in the US or Canada, the median salary of the dataset is 137,570 USD.
* Excluding the US and Canada however, the median salary dropped down to only 69,925 USD.
* Based on experience level, the lowest to highest median salaries goes as follows: Entry-level, Mid-level, Senior-level, Executive.
* Based on employment type, the lowest to highest median salaries goes as follows: Freelancer, Part-timer, Contractor, Full-timer.

### Regression model
* Attempted to create a linear regression model to predict the salary of a given employee in US dollars based on the other features as predictors.
* Unfortunately, the linear model did not work as well as seen in the scatterplot between the predictions of the test set and the true values of the test set. This scatterplot should be a linear line as they error between the prediction values and the true values should not be that great.
* One of the main reasons of why the linear model did not work might be because there are too many outliers in the dataset.
* On top of that, since almost 90% of the dataset is made up of companies that are based in the US or Canada, it might have skewed the training model even more as it does not create a realistic representation of the data.
* Future corrections:
  * Maybe only group the countries as US, Canada, and Others instead.
  * Omit any rows that contain outliers with respect to the salary_in_usd feature.

## Credits
The dataset belongs to Kaggle and can be found in this competition [here](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023).
