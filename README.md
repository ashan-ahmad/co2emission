# CO2 Emission Prediction using Multiple Linear Regression

This project demonstrates the use of **Multiple Linear Regression** to predict CO2 emissions of vehicles based on selected features from a dataset. The dataset used is `FuelConsumption.csv`, which contains model-specific fuel consumption ratings and estimated carbon dioxide emissions for new light-duty vehicles for retail sale in Canada.

## Dataset Description

The dataset includes the following features:
- **MODEL YEAR**: e.g., 2014
- **MAKE**: e.g., VOLVO
- **MODEL**: e.g., S60 AWD
- **VEHICLE CLASS**: e.g., COMPACT
- **ENGINE SIZE**: e.g., 3.0
- **CYLINDERS**: e.g., 6
- **TRANSMISSION**: e.g., AS6
- **FUEL TYPE**: e.g., Z
- **FUEL CONSUMPTION in CITY (L/100 km)**: e.g., 13.2
- **FUEL CONSUMPTION in HWY (L/100 km)**: e.g., 9.5
- **FUEL CONSUMPTION COMBINED (L/100 km)**: e.g., 11.5
- **FUEL CONSUMPTION COMBINED MPG (MPG)**: e.g., 25
- **CO2 EMISSIONS (g/km)**: e.g., 182

The goal is to create a regression model to predict CO2 emissions based on selected features.

## Project Workflow

1. **Data Loading and Exploration**:
   - Load the dataset from a URL.
   - Explore the data using descriptive statistics and random sampling.

2. **Data Cleaning**:
   - Drop irrelevant or redundant features such as `MODELYEAR`, `MAKE`, `MODEL`, etc.
   - Analyze correlations to select the most relevant features.

3. **Feature Selection**:
   - Retain features with high correlation to the target variable (`CO2EMISSIONS`).
   - Drop redundant features like `CYLINDERS` and less correlated fuel consumption metrics.

4. **Data Visualization**:
   - Use scatter plots and scatter matrices to visualize relationships between features and the target variable.

5. **Data Preprocessing**:
   - Standardize the selected features using `StandardScaler`.

6. **Model Training**:
   - Split the data into training and testing sets.
   - Train a multiple linear regression model using the training data.

7. **Model Evaluation**:
   - Evaluate the model's performance on the test data.
   - Visualize the regression plane in 3D and compare predictions with actual values.

8. **Feature-Specific Analysis**:
   - Perform regression analysis for individual features (`ENGINESIZE` and `FUELCONSUMPTION_COMB_MPG`) and visualize the results.

## Key Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`

## Visualizations

- Scatter plots for feature-target relationships.
- 3D regression plane visualization.
- Best-fit regression lines for individual features.

## How to Run

1. Clone the repository.
2. Install the required Python libraries using `pip install -r requirements.txt`.
3. Open the Jupyter Notebook file `CO2_Emission.ipynb`.
4. Run the cells sequentially to execute the project.

## Results

The project demonstrates how to:
- Select relevant features for regression.
- Train and evaluate a multiple linear regression model.
- Visualize the regression results and interpret the model's coefficients.

## Dataset Source

The dataset can be downloaded from [Open Canada](http://open.canada.ca/data/en/dataset/98f1a129-f628-4ce4-b24d-6f16bf24dd64).

## License

This project is licensed under the MIT License. See the LICENSE file for details.
