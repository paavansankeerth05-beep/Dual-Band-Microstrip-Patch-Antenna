# Dual-Band-Microstrip-Patch-Antenna
# Design and Simulation of a Dual-Band Slot-Loaded Microstrip Patch Antenna for 5G Sub-6 GHz and Wi-Fi 6 Applications

![Antenna Geometry]

## 📌 Executive Summary
This repository contains the full CST Studio Suite design, electromagnetic simulation, and performance analysis of a dual-band microstrip patch antenna targeting **3.5 GHz (5G Sub-6 GHz)** and **5.85 GHz (WLAN/Wi-Fi 6)** bands. 

By strategically etching two vertical slots into a rectangular patch on an industry-grade **Rogers AD255C ($\epsilon_r = 2.50$, $h = 1.56\text{ mm}$)** substrate, the antenna achieves dual-band operation with a simplified 2-slot architecture, high radiation efficiency, and superior impedance matching ($S_{11} < -10\text{ dB}$).

---

## 🛠️ Key Design Specifications & Dimensions

* **Substrate Material:** Rogers AD255C ($\epsilon_r = 2.50$, $\tan\delta = 0.0013$)
* **Substrate Dimensions:** $30\text{ mm} \times 30\text{ mm} \times 1.56\text{ mm}$
* **Patch Dimensions:** $15.46\text{ mm} \times 19.38\text{ mm}$
* **Feed System:** $50\ \Omega$ Microstrip Feed Line ($12\text{ mm} \times 4.38\text{ mm}$)
* **Excitation Port:** Waveguide Port (Optimized $k$-factor extension)
* **Conductor Layer:** $0.035\text{ mm}$ (1 oz Copper)

---

## 📊 Performance Summary & Results

### 1. $S_{11}$ & Impedance Bandwidth Performance

![S11 Curve]

| Parameter | Band 1 (5G Sub-6 GHz) | Band 2 (Wi-Fi 6 / WLAN) |
| :--- | :--- | :--- |
| **Resonant Frequency ($f_c$)** | **3.51 GHz** | **5.85 GHz** |
| **Minimum Return Loss ($S_{11}$)** | **$-13.8\text{ dB}$** | **$-17.2\text{ dB}$** |
| **Lower Frequency ($f_L$)** | $3.498\text{ GHz}$ | $5.814\text{ GHz}$ |
| **Upper Frequency ($f_H$)** | $3.525\text{ GHz}$ | $5.901\text{ GHz}$ |
| **$-10\text{ dB}$ Absolute Bandwidth** | **$26.98\text{ MHz}$** | **$86.89\text{ MHz}$** |
| **Fractional Bandwidth (FBW)** | **$0.77\%$** | **$1.48\%$** |

---

### 2. Efficiency, Directivity, and Realized Gain

![Farfield 3.5 GHz]
![Farfield 5.85 GHz]

| Metric | 3.51 GHz Band | 5.85 GHz Band |
| :--- | :--- | :--- |
| **Directivity** | $5.82\text{ dBi}$ | $5.24\text{ dBi}$ |
| **Radiation Efficiency** | $-0.798\text{ dB}$ ($83.21\%$) | $-0.262\text{ dB}$ ($94.14\%$) |
| **Total Efficiency** | $-1.190\text{ dB}$ ($76.03\%$) | $-0.311\text{ dB}$ ($93.09\%$) |
| **Realized Gain** | **$4.63\text{ dBi}$** | **$4.93\text{ dBi}$** |

> **Key Trade-off Analysis:** While both resonances satisfy the $-10\text{ dB}$ matching criterion, the 5.85 GHz band provides significantly higher **Total Efficiency ($93.09\%$)** due to reduced reflection loss and lower dielectric attenuation at higher frequencies.

---

## ⚡ Electromagnetic Field Analysis (Surface Currents)

![Surface Current Comparison]

* **3.51 GHz Resonance:** High surface current density concentrates around the primary center slot (**Slot 1**). The slot forces the current to take a longer electrical detour, pulling down the fundamental frequency.
* **5.85 GHz Resonance:** High current density bypasses the center and shifts heavily toward the offset slot (**Slot 2**) and the outer edges of the patch, providing the shorter effective path needed for the higher frequency mode.

---

## 🛠️ How to Run the Simulation

1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Dual-Band-Microstrip-Patch-Antenna.git](https://github.com/YOUR_USERNAME/Dual-Band-Microstrip-Patch-Antenna.git)
