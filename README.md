# 🏎️ F1 Tyre Degradation & Pit Stop Prediction

This project predicts **F1 lap times** and **pit stop probability** using AI models trained on 2023 Formula 1 race data. It leverages telemetry, tyre, stint, position, and weather data to generate actionable predictions for lap strategy.

---

## 🔹 Features

- **Lap Time Prediction**: Predicts lap times using an XGBoost regression model.
- **Pit Stop Prediction**: Estimates the likelihood of a pit stop next lap using an XGBoost classification model.
- **Input Parameters**: Tyre life, compound type, stint number, driver position, lap time delta, gap to car ahead, track and air temperature, rainfall, humidity.
- **Interactive Gradio App**: Provides an easy-to-use interface for testing predictions.

---

## 📊 Models & Artifacts

- **Lap Time Model**: `tyre_degradation_xgb_model.joblib`  
- **Pit Stop Model**: `pit_stop_predictor_model.joblib`  
- **Encoders**: `compound_encoder.pkl`, `pit_stop_encoder.pkl`  
- **Feature Lists**: `lap_time_features.pkl`, `pit_stop_feature_columns.pkl`  

---

## ⚠️ Notes

- The dataset may contain mixed-type columns; models expect proper types (`str` for `Compound` and `TrackStatus`).  
- Pit stop prediction is imbalanced (few pit stops vs many non-pit laps); probabilities reflect this.  
- Track and weather features are included to improve prediction accuracy.  

---

## 📚 References

- [FastF1 Documentation](https://theoehrly.github.io/Fast-F1/)  
- Formula 1 2023 telemetry data  

---

## 🔗 Author

Ayaan Edward  
Amity University, Noida  
