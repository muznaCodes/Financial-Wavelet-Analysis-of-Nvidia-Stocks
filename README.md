---

# 📈 Time Series Analysis of Financial Trends using Wavelet Transforms

A signal processing-based project that applies **wavelet transforms** to analyze, visualize, and denoise financial time-series data. This project focuses on extracting meaningful insights from stock price data using advanced time-frequency techniques.

---

## 🚀 Overview

Financial time-series data is **non-stationary**, meaning its statistical properties change over time. Traditional methods (like Fourier transforms) fail to capture localized patterns effectively.

This project uses **wavelet transforms** to:

* Analyze stock price behavior across time and frequency
* Detect short-term fluctuations and long-term trends
* Remove noise while preserving important signal characteristics

---

## ✨ Key Features

* 📊 Time-series visualization of stock prices
* 🌊 Continuous Wavelet Transform (CWT) for time-frequency analysis
* 🔍 Zoomed analysis for specific time windows
* 📉 Wavelet entropy for complexity measurement
* 🧹 Discrete Wavelet Transform (DWT) for denoising
* 📈 Comparison of original vs cleaned signals

---

## 🛠️ Technologies Used

* **MATLAB**
* Wavelet Toolbox
* Signal Processing Toolbox

---

## 📂 Dataset

* Historical stock data (CSV format)
* Focus: **Nvidia Corporation** stock prices
* Data includes:

  * Date
  * Adjusted Closing Price

---

## ⚙️ Methodology

The project is divided into modular stages:

---

### 1️⃣ Data Acquisition & Preprocessing

* Import CSV data into MATLAB
* Convert dates into datetime format
* Plot raw time-series

---

### 2️⃣ Continuous Wavelet Transform (CWT)

* Uses **Morlet wavelet (`amor`)**
* Generates a **scalogram (time-frequency representation)**
* Detects:

  * Long-term trends (low frequency)
  * Short-term volatility (high frequency)

---

### 3️⃣ Time-Windowed (Zoomed) Analysis

* Focus on specific date ranges (e.g., Feb–Mar 2023)
* Helps identify localized anomalies and events

---

### 4️⃣ Wavelet Entropy

Used to measure signal complexity:

E = -\sum p_i \log(p_i)

* Higher entropy → more randomness
* Lower entropy → more structured behavior

Also computes:

* Mean of coefficients
* Standard deviation

---

### 5️⃣ Discrete Wavelet Transform (DWT) & Denoising

* Uses **Daubechies-4 (`db4`) wavelet**
* Steps:

  * Decompose signal into approximation & detail
  * Apply soft thresholding
  * Reconstruct denoised signal

---

## 🧩 System Architecture

```
Data Input → CWT Analysis → Zoomed Analysis → Entropy → DWT Denoising
```

Each module is independent, making the system:

* 🔄 Modular
* 📦 Scalable
* 🧪 Easy to test

---

## ▶️ How to Run

### Requirements

* MATLAB (R2023a or later recommended)
* Wavelet Toolbox
* Signal Processing Toolbox

### Steps

1. Open MATLAB
2. Load the dataset (CSV file)
3. Run the main script
4. View:

   * Time-series plots
   * Wavelet spectrograms
   * Denoised signal output

---

## 📊 Results

* ✔️ Clear visualization of stock trends
* ✔️ Effective time-frequency decomposition
* ✔️ Successful noise reduction using DWT
* ✔️ Entropy confirms realistic financial signal complexity

---

## Results

<img width="672" height="395" alt="image" src="https://github.com/user-attachments/assets/0046cf64-a910-4aa4-a1b6-1e5a7553e9a8" />

<img width="688" height="415" alt="image" src="https://github.com/user-attachments/assets/1fe6f3aa-58ea-4d3c-bee3-650f728a5b9c" />



## 📌 Applications

* 📈 Stock market analysis
* 🤖 Preprocessing for ML models
* 📊 Volatility and anomaly detection
* 💹 Financial forecasting research

---

## 🔮 Future Improvements

* Real-time stock data integration
* Machine learning-based prediction models
* Automated anomaly detection
* Interactive dashboards (Python/Streamlit)

---

## 👩‍💻 Author

**Muzna Kamal**
BSEE, National University of Computer & Emerging Sciences (FAST-NUCES), Karachi

---

## 📚 References

* Mallat, *Wavelet Tour of Signal Processing*
* Torrence & Compo, *Wavelet Analysis Guide*
* MATLAB Wavelet Toolbox Documentation

---

## 📜 License

This project is for academic and research purposes.

---
