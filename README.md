# 🎬 CinemaPulse AI — Movie Screening Demand & Revenue Intelligence

**Predicting Cinema Occupancy. Understanding Audience Demand. Optimizing Screening Decisions.**

CinemaPulse AI is a machine learning-powered cinema intelligence system that analyzes movie popularity, audience ratings, genres and screening configurations to predict estimated theatre occupancy, evaluate ticket revenue scenarios and recommend potentially profitable screening schedules.

The project combines real movie metadata and user ratings with a simulated cinema operations dataset to demonstrate an end-to-end Data Science workflow.

---

## 🚀 Project Overview

Cinema operators need to make decisions about:

- Which movies deserve more screening slots?
- Which showtimes could attract higher audiences?
- How might ticket pricing affect estimated revenue?
- Which movie genres show stronger audience interest?
- How can screening configurations be compared systematically?

CinemaPulse AI explores these questions using machine learning, predictive analytics and scenario-based optimization.

## ✨ Key Features

### 1. Movie Intelligence
- Automatic MovieLens dataset integration.
- Movie popularity scoring.
- Genre distribution analysis.
- Average audience rating analysis.
- Movie-level engagement insights.

### 2. Cinema Occupancy Prediction
- Predicts estimated screening occupancy percentages.
- Uses an Extra Trees Regression model.
- Incorporates movie, schedule and operational features.
- Produces predicted occupied seats.

### 3. Revenue Intelligence
- Estimates gross ticket revenue.
- Compares ticket prices.
- Analyzes revenue across different showtimes.
- Evaluates estimated revenue by movie genre.

### 4. Advanced What-If Simulation
- Tests multiple ticket prices.
- Compares different screening times.
- Evaluates occupancy changes.
- Identifies the highest predicted revenue configuration among tested scenarios.

### 5. Screening Schedule Optimization
- Ranks candidate movie screenings.
- Recommends showtimes.
- Compares predicted occupancy and revenue.
- Generates optimized screening reports.

### 6. Model Explainability
- Permutation feature importance.
- Feature importance analysis.
- Actual vs predicted occupancy.
- Demand-category error analysis.

---

## 🧠 Machine Learning Architecture

```text
              MovieLens Dataset
                     |
          ------------------------
          |                      |
      Movies.csv             Ratings.csv
          |                      |
          -----------+------------
                     |
             Movie Data Processing
                     |
          Popularity & Genre Analysis
                     |
          Simulated Cinema Dataset
                     |
              Feature Engineering
                     |
              Train-Test Split
                     |
            Extra Trees Regressor
                     |
          Occupancy Predictions
                     |
       -----------------------------
       |             |             |
    Revenue       What-If       Explainability
   Estimation    Simulation      Analysis
       |             |             |
       -----------+-----------------
                   |
          Screening Optimizer
                   |
           Business Insights
```

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Prediction Model | ExtraTreesRegressor |
| Model Explainability | Permutation Importance |
| Model Persistence | Joblib |
| Dataset | MovieLens |
| Development | Google Colab |

## 📊 Dataset

**MovieLens Latest Small Dataset**

Source: https://grouplens.org/datasets/movielens/latest/

The dataset provides:
- Movie titles
- Movie genres
- User ratings
- Rating counts
- Average ratings

CinemaPulse AI automatically downloads and processes this dataset.

### Important Data Transparency

MovieLens does not provide actual theatre occupancy, screening attendance, ticket prices, ticket sales or cinema revenue.

Therefore, the following variables are simulated for this project:

- Screening occupancy
- Ticket prices
- Theatre capacity
- Marketing expenditure
- Competitor activity
- Holiday indicators
- Estimated ticket revenue

The model is trained and evaluated against simulated occupancy labels. Its evaluation metrics must not be interpreted as validated real-world cinema forecasting accuracy.

---

## ⚙️ Model Development

**Algorithm:** Extra Trees Regressor

The model uses features such as:

- Movie rating count
- Average audience rating
- Rating variability
- Release year
- Movie genre
- Day of the week
- Month
- Showtime
- Weekend and prime-time indicators
- Screen capacity
- Ticket price
- Marketing expenditure
- Competition score
- Holiday indicator
- Days since release

**Target variable:** Screening occupancy percentage.

### Evaluation Metrics

The project evaluates the model using:

| Metric | Purpose |
|---|---|
| MAE | Average absolute prediction error |
| RMSE | Penalizes larger prediction errors |
| R² Score | Measures explained variance |

Actual numerical results are generated when the notebook runs. See `reports/model_metrics.json` for the recorded results.

---

## 📈 Visual Analytics

CinemaPulse AI generates visualizations covering:

1. Top popular movies
2. Movie genre distribution
3. Audience rating distribution
4. Cinema occupancy distribution
5. Average occupancy by genre
6. Average occupancy by showtime
7. Actual vs predicted occupancy
8. Feature importance
9. Permutation feature importance
10. Demand-category prediction error
11. Ticket price versus estimated revenue
12. Optimized screening revenue
13. Estimated revenue by genre
14. Estimated revenue by showtime

---

## 📂 Project Structure

```text
CinemaPulse_AI/
│
├── data/
│   ├── movielens/
│   ├── prepared_movie_data.csv
│   └── simulated_cinema_screenings.csv
│
├── models/
│   └── cinemapulse_occupancy_model.pkl
│
├── outputs/
│   ├── recommended_screening_schedule.csv
│   └── visualizations/
│
├── reports/
│   ├── model_metrics.json
│   ├── actual_vs_predicted.csv
│   ├── feature_importance.csv
│   ├── example_prediction.json
│   └── business_summary.json
│
├── advanced/
│   ├── permutation_feature_importance.csv
│   ├── demand_level_error_analysis.csv
│   ├── what_if_price_simulation.csv
│   ├── optimized_movie_screenings.csv
│   ├── business_decision_report.json
│   └── advanced_project_summary.json
│
└── README.md
```

*The exact files may vary slightly depending on which notebook cells have been executed.*

---

## ▶️ How to Run

1. Open Google Colab.
2. Create a new Python notebook.
3. Copy the complete CinemaPulse AI implementation.
4. Run the main implementation cell.
5. Run the advanced upgrade cell.
6. Allow the MovieLens dataset to download automatically.
7. Explore the generated predictions, visualizations and reports.
8. Download the generated project ZIP.

No manual dataset upload or API key is required.

---

## 🔬 Advanced Business Applications

CinemaPulse AI demonstrates how data-driven decision support could assist cinema operators with:

- Comparing screening configurations.
- Evaluating ticket pricing scenarios.
- Identifying potentially high-demand showtimes.
- Comparing genre-level audience patterns.
- Estimating screening revenue under different assumptions.

These applications would require validation against actual cinema transaction and attendance records before commercial deployment.

---

## 🔮 Future Enhancements

- Integration with real cinema ticket booking data.
- Indian cinema and regional-language movie analytics.
- Real-time ticket sales tracking.
- Actual holiday and festival calendars.
- Multi-screen scheduling optimization.
- Demand forecasting using time-series models.
- Interactive Streamlit dashboard.
- Integration of real theatre capacity and operational costs.

---

## 🎯 Skills Demonstrated

- Exploratory Data Analysis
- Data Cleaning and Feature Engineering
- Regression Modeling
- Model Evaluation
- Feature Importance
- Permutation-Based Explainability
- Scenario Analysis
- Revenue Estimation
- Optimization and Decision Support
- Data Visualization
- Python Project Development

---

## 👨‍💻 Project Information

**Project:** CinemaPulse AI  
**Challenge:** Day 14 — Daily Data Science Project Challenge  
**Domain:** Entertainment Analytics / Machine Learning  
**Environment:** Google Colab  
**Model:** Extra Trees Regressor

---

## ⚠️ Disclaimer

CinemaPulse AI is an educational Data Science portfolio project. MovieLens data is real, while screening-level operational variables and revenue labels are simulated. The generated predictions and optimization recommendations are experimental and should not be treated as actual cinema business forecasts.

**Built to demonstrate how Machine Learning can transform entertainment data into actionable business insights.**
