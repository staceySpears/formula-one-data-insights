# Formula One Data Insights

## Project Overview
This project aims to develop a predictive model to understand the impact of race
location on race finish positions. By analyzing historical race data, we seek to
provide insights and improve predictive accuracy for race outcomes.

## Repository Structure

formula-one-data-insights/
├── F1_cleaned_data/
├── F1_visuals/
│   ├── correlation_matrix.png
│   ├── boxplot_finish_positions.png
│   ├── distribution_of_points.png
│   ├── average_race_position_over_years.png
│   ├── grid_vs_final_position.png
│   ├── confusion_matrix.png
│   ├── feature_importance.png
│   └── shap_summary_plot.png
├── notebooks/
│   ├── data_preprocessing_and_eda.ipynb
│   ├── model_building_and_evaluation.ipynb
└── README.md

## Data Preprocessing
- Filled missing values using the forward fill method.
- Dropped unnecessary columns such as 'time_x' and 'time_y'.
- Ensured numeric values in key columns like 'fastestLapSpeed' and 'laps'.
- Handled remaining NaNs by filling them with appropriate values (e.g., mean).

## Exploratory Data Analysis (EDA)
- Generated a correlation matrix to identify relationships between variables.
- Visualized the distribution of finish positions across different circuits using
  a boxplot.
- Analyzed the distribution of points scored by drivers.
- Conducted a time series analysis of average race positions over the years.
- Explored the relationship between grid positions and final race positions.

## Feature Engineering
- Created additional features such as `race_circuit_date`, `average_speed`,
  `driver_experience`, `driver_wins`, `constructor_points`, `constructor_wins`,
  and `historical_performance_circuit`.

## Model Building and Evaluation
- Built and tuned a Random Forest model using GridSearchCV.
- Compared the performance of the Linear Regression and Random Forest models
  based on Mean Absolute Error (MAE).
- The Random Forest model was chosen as the champion model due to its superior
  prediction accuracy.

## Visualizations
- ![Correlation Matrix](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/correlation_matrix.png?raw=true)
- ![Boxplot Finish Positions](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/boxplot_finish_positions.png?raw=true)
- ![Distribution of Points](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/distribution_of_points.png?raw=true)
- ![Time Series Analysis](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/average_race_position_over_years.png?raw=true)
- ![Grid vs Final Position](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/grid_vs_final_position.png?raw=true)
- ![Confusion Matrix](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/confusion_matrix.png?raw=true)
- ![Feature Importance](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/feature_importance.png?raw=true)
- ![SHAP Summary Plot](https://github.com/staceySpears/formula-one-data-insights/blob/main/F1_visuals/shap_summary_plot.png?raw=true)

## Conclusion
The chosen champion model is the Random Forest model with the lowest Mean
Absolute Error, demonstrating superior prediction accuracy. This model can be
used to guide recruitment decisions effectively by predicting race outcomes
based on historical data.

## Next Steps
- Further refine the model by incorporating additional features and data.
- Explore other advanced machine learning techniques to improve predictive
  accuracy.
- Use the insights from this analysis to inform strategic decisions in the
  context of Formula One racing.
