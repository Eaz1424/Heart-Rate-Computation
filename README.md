# Heart Rate Computation

This project demonstrates ECG (Electrocardiogram) signal processing for detecting R-peaks and calculating the average heart rate. It utilizes sample ECG data and provides a comprehensive pipeline for signal filtering, peak detection, and heart rate computation.

## Table of Contents
- [Overview](#overview)
- [Files in the Repository](#files-in-the-repository)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Details on ECG Signal Processing](#details-on-ecg-signal-processing)
- [License](#license)

---

## Overview

Heart Rate Detection processes ECG signals and detects R-peaks using MATLAB. The project uses two sample datasets to demonstrate the functionality.

It includes:
1. Data filtering to remove noise.
2. Identification of R-peaks using a sliding window algorithm.
3. Visualization of ECG signals and detected peaks.
4. Calculation of the average heart rate based on detected peaks.

## Files in the Repository

1. **`ecgdemo.m`**
   - Main script for ECG processing and heart rate calculation.
   - Demonstrates signal filtering, peak detection, and visualization.
   - Includes plots for various stages of ECG processing.

2. **`ecgdemowinmax.m`**
   - Sliding window-based filtering script for detecting R-peaks in the ECG data.

3. **`ecgdemodata1.mat`**
   - First sample dataset containing ECG signal data.

4. **`ecgdemodata2.mat`**
   - Second sample dataset containing ECG signal data.

5. **`README.md`**
   - This documentation file.

---

## Setup Instructions

### Prerequisites
- MATLAB installed on your system.

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/Eaz1424/Heart-Rate-Detection.git
   ```
2. Open MATLAB.
3. Set the repository directory as the working directory.

---

## Usage

1. Ensure the following files are in the MATLAB workspace folder:
   - `ecgdemo.m`
   - `ecgdemowinmax.m`
   - `ecgdemodata1.mat`
   - `ecgdemodata2.mat`

2. Run the following command in MATLAB's command window:
   ```matlab
   >> ecgdemo
   ```

3. The script will:
   - Process the ECG data samples.
   - Display plots for different stages of ECG signal processing.
   - Output the calculated average heart rate.

---

## Details on ECG Signal Processing

### Steps in Processing
1. **Low-Frequency Noise Removal:**
   - Uses FFT to remove low-frequency components from ECG signals.

2. **Sliding Window Filtering:**
   - Detects R-peaks using a window-based approach.

3. **Heart Rate Calculation:**
   - Computes the average heart rate based on the detected R-peaks.

### Sample Outputs
The script generates visualizations for:
- The original ECG signal.
- Filtered ECG signals.
- Detected R-peaks.
- Final processed ECG with marked R-peaks.
- You will get two figures everyone of which has 6 plots:
  - **First Plot**: Shows the original ECG data.
  - **Second Plot**: Contains corrected ECG data with the low-frequency component removed.
  - **Third Plot**: Shows data after the first filtering pass, where the filter window has default size (results may not be clear).
  - **Fourth Plot**: Displays detected peaks; some peaks may be skipped at this stage.
  - **Fifth Plot**: Results of the second filtering pass after window size optimization.
  - **Sixth Plot**: Final result showing the detected peaks.

---


---
