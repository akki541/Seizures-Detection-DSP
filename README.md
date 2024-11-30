# Seizures Detection using EEG Signals

This project focuses on detecting epileptic seizures from EEG signals using advanced signal processing techniques. The approach includes preprocessing EEG data with filtering methods, frequency domain analysis, and statistical analysis to differentiate between seizure and non-seizure states effectively.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Methodology](#methodology)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [Future Enhancements](#future-enhancements)
- [Contributors](#contributors)
- [License](#license)

---

## Introduction
Epileptic seizures are caused by abnormal electrical discharges in the brain. Electroencephalography (EEG) signals provide a way to monitor these discharges. This project utilizes DSP techniques for detecting seizure activity in EEG signals, aiming to support real-time diagnosis.

---

## Features
- **Signal Preprocessing**: Removal of noise and artifacts using a low-pass FIR filter with Kaiser window.
- **Frequency Analysis**: Fast Fourier Transform (FFT) for identifying significant frequency patterns in EEG signals.
- **Statistical Analysis**: Use of mean and standard deviation to analyze EEG signal variability for seizure detection.
- **Visualizations**: Time-domain and frequency-domain plots for signal interpretation.

---

## Methodology
1. **Data Acquisition**:
   - EEG signals are sourced from publicly available datasets.
   - Signals are filtered to remove frequencies outside the 0–30 Hz band.

2. **Signal Filtering**:
   - FIR low-pass filter with Kaiser window to enhance signal quality.

3. **Frequency Domain Analysis**:
   - Application of FFT to convert EEG signals into the frequency domain and identify seizure-specific frequency components.

4. **Statistical Analysis**:
   - Statistical parameters, such as mean and standard deviation, are computed to detect variability in EEG signals.

5. **Visualization**:
   - Plots are generated to compare seizure and non-seizure signals in both time and frequency domains.

---

## Requirements
- Python 3.x
- NumPy
- Matplotlib
- SciPy

Install the dependencies using:
```bash
pip install -r requirements.txt
