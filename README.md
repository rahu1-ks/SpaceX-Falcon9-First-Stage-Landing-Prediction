
# SpaceX Falcon9 First Stage Landing Prediction

## Project Overview

This project aims to predict the successful landing of the first stage of the Falcon 9 launch vehicle (LV) developed by SpaceX. Successful landings are critical as they significantly reduce launch costs by enabling the reuse of the first stage. By predicting whether the first stage will successfully land, we can estimate the overall launch cost, providing valuable insights into space transport economics.

## Problem Statement

SpaceX's Falcon 9 is a reusable, two-stage rocket designed for space transport. The ability to successfully land the first stage of the rocket enables SpaceX to offer significantly lower launch costs compared to competitors. The main goal of this project is to predict the landing outcome of the first stage of Falcon 9 based on several factors such as payload, launch site, orbit type, and more.

## Data Collection

The data used for this project was sourced from:
- **SpaceX REST API**: Provided information on flight numbers, launch dates, booster versions, payload mass, orbit type, launch sites, and landing outcomes.
- **Web Scraping**: Data from Wikipedia including additional details such as customers, landing outcomes, and booster landing specifics.

## Methodology

1. **Data Wrangling**:
   - Data was cleaned and processed to handle missing values.
   - One-hot encoding was used to transform categorical data into numerical format for model training.

2. **Exploratory Data Analysis (EDA)**:
   - EDA was conducted using SQL queries to analyze key factors such as payload mass, orbit type, launch sites, and landing outcomes.
   - Scatter plots, bar charts, and line charts were generated to visualize relationships between variables.
   - Interactive maps and dashboards were created using Folium and Plotly Dash to explore geographical factors influencing landing success.

3. **Predictive Analysis**:
   - Several machine learning models were implemented, including Decision Tree, Random Forest, and Logistic Regression, to predict landing outcomes.
   - Hyperparameter tuning was conducted using GridSearchCV to improve model performance.
   - The models were evaluated based on accuracy, and a confusion matrix was used to assess the best-performing model.

## Key Results

- The **Decision Tree Classifier** was the best-performing model, achieving the highest accuracy.
- Flight success rates increased significantly from 2013 to 2020, with **KSC LC-39A** being the most successful launch site.
- Orbits such as ES-L1, GEO, HEO, SSO, and VLEO had the highest success rates.
- Higher success rates were observed with payloads in the 1900 kg to 5000 kg range.

## Visualizations

- **Interactive Maps**: Displays launch sites and success/failure markers.
- **Dashboards**: Provides detailed insights on success rates based on payload mass, orbit, and launch site.

## Conclusion

This project successfully predicted the landing outcome of Falcon 9's first stage with high accuracy using a Decision Tree classifier. The model can be further optimized and used by SpaceX or similar companies to predict landing outcomes for future launches, ultimately contributing to cost savings and more efficient space transportation.


## License

This project is licensed under the MIT License.

---

**References**:
- SpaceX REST API
- Wikipedia
