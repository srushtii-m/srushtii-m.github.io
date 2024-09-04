---
title: "Advanced Graph-Based Deep Learning for Predictive Analytics in Urban Bike-Sharing Systems"
excerpt: "This study leverages advanced graph convolutional networks to accurately predict bike demand, incorporating complex spatial and temporal dynamics to enhance the efficiency and reliability of urban bike-sharing systems."
collection: portfolio1
---

Bike-sharing systems like Citi Bike offer flexible and environmentally friendly travel options in urban areas. However, their effectiveness depends on accurately predicting bike demand, which is influenced by factors such as weather, urban events, and commuter habits. My independent study at the University of Illinois Urbana-Champaign, under the guidance of Ujjal K Mukherjee, aimed to address this challenge by applying advanced graph-based deep learning techniques to enhance the predictive analytics of bike-sharing systems.

## Problem Statement

Predicting bike demand in urban bike-sharing systems presents significant challenges due to the dynamic and non-linear nature of usage patterns. Traditional forecasting methods often fail to capture the complex spatial and temporal interdependencies between bike stations. Existing models do not fully exploit the spatial interconnections between stations nor adapt to the temporal variations in bike usage, leading to inefficient resource allocation and user dissatisfaction. My study focuses on overcoming these limitations by integrating spatial and temporal dynamics into a coherent predictive model without excessive computational demands.

## Objectives

This study aims to implement and evaluate three different models based on advanced graph convolutional networks (GCNs) to predict traffic flows accurately. The objectives are:
1. To adapt and evaluate the efficacy of Spatio-Temporal Graph Convolutional Networks (STGCN) for modeling the complex spatio-temporal relationships inherent in bike-sharing demand.
2. To implement Attention Based Spatial-Temporal Graph Convolutional Networks (ASTGCN) with an emphasis on their ability to prioritize key spatial and temporal features critical for predicting bike demand fluctuations.
3. To explore the capabilities of a third model, focusing on its specialized handling of dynamic spatial-temporal correlations, for its suitability in predicting bike station demand under varying urban conditions.
4. To compare the performance of these models using Mean Absolute Error (MAE) and other relevant metrics, aiming to identify which model best captures the dynamics of bike demand.
5. To determine the practical implications of these findings for real-time bike-sharing management and suggest directions for future enhancements in predictive modeling techniques.

## Methodology

The study utilized data from NYC Citi Bike Rentals, which included features such as start and end station names, ride types, dates, times, trip durations, locations, weather conditions, user types, and demographics. The data underwent thorough cleaning and preprocessing, including time-series analysis to identify patterns and trends. Key steps in the time-series analysis included:

- **Seasonal Decomposition:** Revealed annual cyclic trends in the data.
- **Autocorrelation and Partial Autocorrelation Plots:** Identified significant patterns indicating dependencies within the data.
- **Dickey-Fuller Test:** Confirmed the stationarity of the dataset, showing consistent patterns over time.
- **Variance Inflation Factor (VIF):** Addressed multicollinearity concerns through feature selection, improving model robustness.

### Three models were implemented:

1. **Spatio-Temporal Graph Convolutional Networks (STGCN):** This model captures spatial and temporal dependencies through graph convolutions and gated temporal convolutions.
2. **Attention Based Spatial-Temporal Graph Convolutional Networks (ASTGCN):** This model incorporates attention mechanisms to dynamically focus on important spatial and temporal features.
3. **Spatio-Temporal Neural Structural Causal Models (STNSCM):** This model integrates causal reasoning and counterfactual analysis to improve the robustness and adaptability of predictions.

## Results

1. **STGCN Model:** Demonstrated a Mean Absolute Error (MAE) of 0.767 bikes and a Root Mean Square Error (RMSE) of 1.182 bikes, indicating a moderate level of prediction accuracy.
2. **ASTGCN Model:** Achieved a Mean Absolute Error (MAE) of 0.96, showing high accuracy in forecasting demand across different stations and times.
3. **STNSCM Model:** Showed an MAE of 2.67 when considering contextual features, suggesting strong performance in integrating external influences.

## Conclusion

The study's findings highlight the effectiveness of advanced graph convolutional networks in predicting bike-sharing demand. Each model demonstrated unique strengths in handling spatial and temporal data complexities, with the STGCN and ASTGCN models providing notable improvements in prediction accuracy. The integration of causal reasoning in the STNSCM model further enhanced the robustness of predictions, especially under varying conditions.

Future research could explore the integration of these models with real-time data and the inclusion of additional variables such as weather conditions and special events. This approach could significantly improve the accuracy and reliability of predictive models, contributing to better management and planning of urban bike-sharing systems.

For a detailed exploration of the methodologies and results, you can refer to the full codes [here](https://github.com/srushtii-m/Citibike-Demand-Prediction-Using-GCN-s).