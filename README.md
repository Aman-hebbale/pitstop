# 🏎️ F1 Pit Stop Analysis — Monza 2024

This project performs a data analysis of Formula 1 pit stops from the 2024 Italian Grand Prix at Monza. The analysis uses the [`FastF1`](https://theoehrly.github.io/Fast-F1/) library to retrieve session data and utilizes Python's data science ecosystem for processing and visualization.

## 📁 Project Structure

- `pit-stop-analysis.ipynb`: Jupyter notebook with the complete analysis pipeline.
- `monza_2024.csv`: CSV export of lap-by-lap data from the Monza 2024 race session (generated during the notebook execution).

## 🚀 Features

- Loads and caches Formula 1 telemetry and lap data using FastF1.
- Extracts and saves lap data to a CSV file.
- Prepares for detailed analysis of pit stops.

## 🧪 Feature Engineering

The project extracts raw lap-by-lap telemetry data and derives new features to enable strategic analysis:

- **Pit Lap Identification**: Detects laps where drivers entered the pit.
- **Stint Metrics**: Calculates number of laps per stint and duration between stops.
- **Tyre Strategy Sequencing**: Tracks compound usage across stints.
- **Driver-level Aggregation**: Summarizes lap-wise performance into driver-level stats.

These features provide the foundation for evaluating pit strategies and performance impact.

## 🧹 Data Cleaning

While not explicitly shown, typical cleaning tasks likely included:

- **Handling Missing Values**: Removing incomplete or missing telemetry for certain laps.
- **Filtering Non-Racing Laps**: Excluding formation, safety car, or red-flag laps depending on context.
- **Standardization**: Ensuring consistency in data formatting, such as time and driver labels.

Cleaning ensures that insights drawn from the data are accurate and representative.

## 🔮 Predictive Analysis (Potential)

This project sets the stage for future predictive work. Possible extensions include:

- **Pit Stop Prediction**: Forecasting pit windows based on tyre wear and stint length.
- **Strategy Simulation**: Evaluating 1-stop vs. 2-stop strategies under different conditions.
- **Race Outcome Forecasting**: Estimating final positions or position changes after pit stops.
- **Strategy Clustering**: Grouping similar pit strategies using unsupervised learning.

These directions would require integrating labeled outcome data and applying machine learning models.

## 🛠️ Technologies Used

- Python
- FastF1
- Pandas
- Matplotlib
- Seaborn
- NumPy

## 📦 Setup Instructions

1. **Clone the repository** or download the notebook.
2. **Install dependencies**:
   ```bash
   pip install matplotlib seaborn pandas numpy fastf1
