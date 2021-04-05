# Wind-Energy-Prediction
#### Exploration of the Wind. Forecasting surplus and potential energy in the next 24hours. ####

![image](https://user-images.githubusercontent.com/79764958/109397342-06888980-792e-11eb-81ce-fe4d0215b028.png)

This project aims to provide Machine Learning tools to predict Wind Electricity in the island of Irelang for the next 24 h.
The goal will be to present predictions every day at 21:00, if and when (what Hours) will the ratio of Wind generated electricity reaches the currently supported maximum (70%): 
- Predict Wind Electricity hourly generation for the next 24h .
- Compare to predicted demand as per Eirgrid Smartgriddashboard.eirgrid.com 
- Highlighlight hours where Wind generations is higher than 70% demand: manually set up battery charging for those hours!

The following Colabs implement loading relevant data from Met.ie and smartgriddashboard.eirgrid.com , handle missing data and outliers, merge the data into 1 feature vector, try a few different Machine Learning with relevant feature engineering options, and forecast for the next day!

| File | Purpose |
|------|--------|
| 1_weather_data_prep.ipynb | Load Hourly Met.ie data for 4 weather stations for the last 4 years and merge into 1 file|
| 2_IslandElectricityData_ver2.ipynb | Load smartgriddashboard.eirgrid.com electricity generation data for the island of Ireland for the last 4 years |
| 2b_IslandElectricityMissingData.ipynb | Handle missing data in Eirgrid Electricity data |
| 2c_IrelandElectricityDataQualityCheck.ipynb | Compare SEAI monthly summary and Eirgrid data for the Republic of Ireland to check data quality | 
| 3_Krystian's_EDA_SharedIslandElectricityEDAipynb.ipynb | EDA |
| 4_IslandElectricityANNModel_v2.ipynb | Neural Netwok models with transformed features | 
| 4_IslandElectricityRandomForestModel.ipynb | Random Forest model with raw features | 
| 4_IslandElectricityRandomForestModel_transformedTime.ipynb | Random Forest model with transformed features |
| 4_IslandElectricity_autoreg.ipynb | AutoReg prediction model | 
| Feature Vector - Dictionary - Feature.csv | Feature vector doc for all loaded features |




