# Analog Noise Cancellation PCB with I2S Audio Output

##  Overview

This project presents a custom-designed PCB for an **Analog Noise Cancellation (ANC) system**.
The design uses dual microphones to capture **desired voice** and **ambient noise**, and processes them through an analog front-end using operational amplifiers to suppress noise before digitization.

The filtered analog signal is then fed into an **audio codec**, which converts it into a digital I2S stream for further processing by a processor or FPGA.

---

##  System Architecture

1. **Primary Microphone (Voice Input)**
   Captures the desired speech signal.

2. **Secondary Microphone (Noise Reference)**
   Captures environmental noise.

3. **Analog Processing (Op-Amp Stage)**

   * Signal conditioning
   * Phase inversion of noise signal
   * Summation for noise cancellation

4. **Audio Codec**

   * Converts analog signal → digital
   * Outputs via I2S protocol

5. **Digital Interface (I2S Output)**

   * Connected to processor / FPGA for further processing

---

##  Working Principle

The system is based on **destructive interference**:

* The noise signal is inverted using an op-amp.
* The inverted noise is summed with the original signal.
* Ideally, noise components cancel out, leaving clean voice.

---

##  Features

* Dual-microphone input (voice + noise reference)
* Analog noise cancellation using op-amps
* Pre-digitization noise suppression
* I2S digital audio output
* Compatible with FPGA / embedded processors
* Low-latency processing (pure analog front-end)

---

##  Hardware Components

* Operational Amplifiers (Op-Amps)
* Dual Microphones
* Audio Codec (I2S compatible)
* Passive Components (Resistors, Capacitors)
* Power Supply Regulation Circuit

---

##  Interfaces

* **Analog Inputs:**

  * Mic 1 (Voice)
  * Mic 2 (Noise)

* **Digital Output:**

  * I2S (BCLK, LRCLK, DATA)

---

## 🛠️ Tools Used

* PCB Design: KiCad 


---



---

## 👤 Author

**Manoj R**
Electronics and Communication Engineering

---
Top Layer Layout
<img width="646" height="716" alt="image" src="https://github.com/user-attachments/assets/debcce1d-d68a-4466-a2d9-4322be90dee4" />

Bottom Layer Layout

<img width="569" height="688" alt="image" src="https://github.com/user-attachments/assets/6c56b42c-d935-4202-ad99-918be46e8784" />



