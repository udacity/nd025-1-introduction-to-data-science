# Introduction to Data Science Course

Content for Udacity's Introduction to Data Science course.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>. Please refer to [Udacity Terms of Service](https://www.udacity.com/legal) for further information.

## Survey Data Analysis

This project analyzes survey data from a CSV file (`survey_results_public.csv`) to provide insights into various aspects of the respondents, including their professional status, education, country of origin, employment status, salary expectations, and survey responses. The analysis includes visualizations such as bar charts and pie charts to present the findings clearly.

## Requirements

To run this project, you will need the following Python packages:
```
- `numpy`
- `pandas`
- `matplotlib`
- `ALookAtTheData` (a custom module)
```
You can install the required packages using pip:

```bash
pip install numpy pandas matplotlib
```
Usage
1- Load the Data: The survey data is loaded from a CSV file using pandas.

2- Data Inspection: The first few rows of the dataset are displayed to understand its structure.

3- Data Validation: The number of rows and columns in the dataset is checked to ensure correctness.

4- Missing Values Analysis: The code identifies columns with no missing values and those with more than 75% missing values.

5- Data Visualization:

 - Bar Charts: The following bar charts are generated:
  1- Proportion of individuals in each professional category.
  2- Proportion of individuals based on their formal education.
  3- Proportion of individuals from the top 10 countries.
  4- Proportion of individuals based on their employment status.
 - Salary Analysis: A combined bar chart displays the top 10 salary values and their corresponding salary expectations.
 - Survey Responses: Pie charts visualize the responses to various survey questions.

Code Explanation
The main components of the code are as follows:

- Data Loading: The dataset is loaded using pd.read_csv().
- Data Inspection: The shape of the DataFrame is checked to ensure it has the expected number of rows and columns.
- Missing Values: The code identifies columns with no missing values and those with a significant amount of missing data.
- Value Counts: The code calculates the counts for various categorical columns, such as Professional, FormalEducation, Country, and EmploymentStatus.
- Visualization:
   1- Bar charts are created for categorical data using the plot() method.
   2- A combined bar chart for salary and salary expectations is generated, with values displayed on top of the bars.
   3- Pie charts are created for survey responses, with legends to avoid label overlap.

Example
To run the analysis, simply execute the script in a Jupyter Notebook or any Python environment that supports the required libraries. Ensure that the survey_results_public.csv file is in the same directory as the script.

```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import ALookAtTheData as t
from IPython import display
from matplotlib.ticker import FuncFormatter

# Load the dataset
df = pd.read_csv('./survey_results_public.csv')
df.head()

# Further analysis and visualization code...
```

Conclusion
This project provides a comprehensive analysis of survey data, offering insights into the demographics and opinions of respondents. The visualizations help in understanding the data better and can be used for further analysis or reporting.

License
This project is licensed under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License. This license allows others to download the work and share it with others as long as they credit the author, but they cannot change it in any way or use it commercially. For further details, refer to the Udacity Terms of Service.