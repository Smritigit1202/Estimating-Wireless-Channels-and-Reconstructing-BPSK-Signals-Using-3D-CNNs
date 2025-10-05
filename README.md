

# Deep Learning-Based Wireless Channel Estimation and BPSK Signal Recovery

## Overview

This project uses **Deep Learning**, specifically a **3D Convolutional Neural Network (3D-CNN)**, to estimate wireless channel effects and reconstruct digital signals transmitted using **BPSK (Binary Phase Shift Keying)**. Wireless signals often get distorted due to noise, fading, or interference. Traditional methods can handle some distortions, but they may fail in complex real-world conditions.

Our approach is **data-driven**: the model learns how to recover the original signal from distorted versions, improving accuracy and reliability.

---

## Key Features

* **Signal Reconstruction:** Recovers clean in-phase (I) and quadrature (Q) components from noisy, faded signals.
* **Channel Estimation:** Learns the wireless channel effects automatically using training data.
* **Performance Metrics:** Evaluates results using NMSE (Normalized Mean Squared Error), BER (Bit Error Rate), waveform accuracy, and EVM (Error Vector Magnitude).
* **Generalization:** Can handle varying noise levels and fading patterns.

---

## How It Works

1. Generate or load a dataset of BPSK signals affected by simulated channel impairments.
2. Train a **3D-CNN** on the dataset to map distorted signals to their original clean signals.
3. Evaluate the model on unseen test data using standard metrics.
4. Save reconstructed signals and plots for analysis.

---

## Folder Structure

* `dataset_fixed.xlsx` → Input dataset (received + target signals)
* `reconstructed_outputs/` → Predicted signals by the model
* `reconstructed_plots/` → Plots comparing original vs reconstructed waveforms
* `notebook.ipynb` → Python/Colab notebook containing the code

---

## Requirements

* Python 3.x
* NumPy, Pandas, Matplotlib
* PyTorch
* Openpyxl (for Excel file handling)

---

## Conclusion

This project demonstrates that deep learning can **complement traditional wireless signal processing**, providing a robust way to estimate channels and recover high-fidelity BPSK signals even under noisy and fading conditions.

