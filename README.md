This project is a tutorial assignment completed as part of the AI in Healthcare course during my master's studies. It demonstrates how to use Facebook Prophet for predicting ventilator usage trends in ICU patients using the MIMIC-III clinical dataset.

📚 Project Overview
The goal of this project is to forecast the future demand for ventilators in ICU settings using time-series analysis. By identifying trends and patterns in past ventilator usage, hospitals can better plan and allocate critical care resources.

🏥 Dataset Details
Source: MIMIC-III Clinical Database

Tables Used:

CHARTEVENTS.csv: ICU charted data including ventilator usage

D_ITEMS.csv: Metadata for item IDs

Focus: Extract ventilator-related event records based on item descriptions

Sample Range: Data filtered for the year 2167 for demonstration

⚙️ Methodology
🔄 Data Preprocessing
Filter CHARTEVENTS using ventilator-related itemids

Group data by subject_id to get daily usage counts

Format time-series data as required by Prophet (ds and y columns)

📈 Forecasting with Facebook Prophet
Apply Facebook Prophet to model and forecast future ventilator demand

Tune model parameters for improved accuracy:

seasonality_mode

changepoint_prior_scale

fourier_order

Logistic cap values (for limiting long-term trends)

Visualize forecasts with confidence intervals

