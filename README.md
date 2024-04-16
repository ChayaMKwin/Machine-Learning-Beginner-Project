# Medal Prediction Analysis

## Code Explanation

### 1. Data Loading and Preprocessing
- Load the dataset (`teams.csv`) into a Pandas DataFrame.
- Clean the data by selecting relevant columns and dropping rows with missing values.

### 2. Correlation Analysis
- Compute correlation coefficients between the `medals` column and other numerical columns (`year`, `athletes`, `age`, `prev_medals`) in the dataset.

### 3. Data Visualization
- Create a pair plot using Seaborn to visualize relationships between different numerical variables.
- Plot a scatter plot (`lmplot`) to visualize the relationship between `athletes` and `medals`.

### 4. Model Training and Prediction
- Split the dataset into training (`train`) and test (`test`) sets based on the year.
- Train a linear regression model (`LinearRegression`) using `athletes` and `prev_medals` as predictors and `medals` as the target.
- Make predictions using the trained model on the test set.

### 5. Evaluation
- Calculate Mean Absolute Error (MAE) between predicted and actual `medals` values on the test set.
- Analyze errors and error ratios by team to assess model performance.

## Results

The model predicts Olympic medal counts with a Mean Absolute Error (MAE) of approximately 3.3 medals per team. Further analysis includes error calculation and ratio by team, allowing us to assess prediction accuracy across different countries.
