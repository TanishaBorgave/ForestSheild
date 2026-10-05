# 🌲 ForestShield

### Forest Fire Risk Prediction using Satellite Data and Machine Learning

ForestShield is a machine-learning project for analyzing and predicting fire risk across geographic regions using satellite-based fire observations and environmental data.

The project processes NASA FIRMS VIIRS satellite fire detections, converts individual detections into spatial grid-cell/day fire events, and prepares the data for weather-based fire-risk modeling.

---

## 📌 Overview

Forest fires are influenced by environmental conditions such as temperature, humidity, wind speed, and precipitation.

ForestShield uses historical satellite fire observations to identify where and when fire events occurred and represents the observations on a geographic grid.

The core data pipeline is:

```text
NASA FIRMS VIIRS Data
        ↓
Data Cleaning
        ↓
Confidence Filtering
        ↓
Vegetation Fire Filtering
        ↓
Coordinate Validation
        ↓
Spatial Grid Assignment
        ↓
Daily Grid-Cell Fire Labels
        ↓
Fire Risk Modeling
