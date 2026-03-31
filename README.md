# QPSK-Simulation
Running code for qpsk and bit error rate


# **Introduction**

Digital communication systems rely on modulation techniques that efficiently transmit information over noisy channels. Among these techniques, **Quadrature Phase Shift Keying (QPSK)** is widely used because it offers a strong balance between bandwidth efficiency and error performance. To evaluate how well QPSK performs under different noise conditions, engineers often use **Bit Error Rate (BER) simulations** and compare them with theoretical predictions.  

This program implements a **Monte‑Carlo simulation** of QPSK transmission over an **Additive White Gaussian Noise (AWGN)** channel. It generates random binary data, modulates it into QPSK symbols, adds controlled noise based on varying **Eb/N0** values, and then demodulates the received signal to measure the resulting bit errors. By plotting both the **simulated BER** and the **theoretical BER**, the code provides a clear visualization of QPSK performance and validates the accuracy of the modulation and detection process.



# **Summary of the Code**

This MATLAB program simulates the **Bit Error Rate (BER)** performance of **QPSK modulation** over an **AWGN channel** and compares the results to the **theoretical BER curve**.

### **What the code does:**

- **Generates random bits** for transmission.
- **Maps the bits to QPSK symbols** using a custom modulation function.
- **Adds AWGN noise** to the transmitted symbols at different **Eb/N0 values** (0 to 20 dB).
- **Demodulates** the noisy QPSK symbols back into bits.
- **Counts bit errors** to compute the **simulated BER**.
- **Calculates the theoretical BER** for QPSK using the erfc formula.
- **Plots both curves** (theoretical vs. simulated) on a semilog graph.
- **Saves the results** to a file.

