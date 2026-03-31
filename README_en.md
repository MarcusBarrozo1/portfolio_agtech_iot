# IoT Agricultural Sensor Data Analysis and Processing 🚜

This project presents a basic data cleaning and preparation pipeline for IoT sensor time series in an AgTech context. The main focus was to ensure data integrity before applying machine learning models, simulating real-world hardware and connectivity challenges in the field.

## 🛠️ Technologies and Tools
- **Python 3.x**
- **Pandas & NumPy**: Data manipulation and linear algebra.
- **Matplotlib**: Trend visualization (Dataviz).
- **VS Code & Jupyter Notebooks**: Development environment.

## 📈 Technical Challenges Overcome

### 1. Time Series Management
- Conversion of data types (`object` to `datetime`) and structuring time indexes for accurate chronological analysis.

### 2. Missing Data Imputation (NaN)
- Identification of gaps caused by connectivity failures.
- Application of **Linear Interpolation** to restore the physical continuity of temperature and humidity variables while preserving data coherence.

### 3. Anomaly Detection and Correction (Outliers)
- Implementation of statistical logic based on **Z-Score** (3 standard deviations).
- Automatic identification of unrealistic hardware spikes and replacement with statistically acceptable values through smoothing techniques.

### 4. Feature Engineering
- Implementation of **24-hour Moving Averages (Rolling Window)** to reduce noise and extract long-term climate trends.

## 📊 Results
The project produced a clean dataset (`iot_agricola_clean.csv`), ready for predictive modeling, with visualizations that demonstrate noise removal and daily pattern identification.

---
**Marcus Barrozo** *Geographic Data Scientist | Remote Sensing Specialist*