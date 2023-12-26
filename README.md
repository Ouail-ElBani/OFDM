# OFDM Simulation

## Overview
This MATLAB script simulates a simple Orthogonal Frequency Division Multiplexing (OFDM) system. OFDM is a widely used technique in modern communication systems for transmitting data over multiple subcarriers efficiently. The provided script demonstrates the basic steps involved in an OFDM communication system, including data generation, modulation, channel transmission with additive white Gaussian noise (AWGN), and reception with decoding.

## Script Details

### Parameters
- `N`: Number of subcarriers in the OFDM system.
- `SNR_dB`: Signal-to-Noise Ratio in decibels for the AWGN channel.

### Data Generation and Modulation
1. Generate random binary data (BPSK modulation) for transmission.
2. Modulate the binary data using Binary Phase Shift Keying (BPSK) modulation.

### OFDM Symbol Generation
1. Perform a Discrete Fourier Transform (FFT) on the modulated data to convert it into the frequency domain.
2. Add cyclic prefixes to create the OFDM symbol.

### Channel Transmission
1. Simulate transmission through an AWGN channel.
2. Display the transmitted OFDM signal.

### Reception and Demodulation
1. Remove the cyclic prefixes from the received signal.
2. Perform an Inverse FFT (IFFT) to convert the received signal back to the time domain.
3. Demodulate the received signal to obtain the decoded data.

### Error Analysis
1. Calculate the Binary Error Rate (BER) by comparing the decoded data with the original transmitted data.
2. Display the received OFDM signal and the decoded data.

## Running the Script
1. Open MATLAB.
2. Copy and paste the script into the MATLAB editor.
3. Modify the parameters if needed.
4. Run the script.

## Results
The script generates two figures:
1. Figure 1: Shows the original data to be transmitted and the transmitted OFDM signal.
2. Figure 2: Displays the received OFDM signal and the decoded data.

The Binary Error Rate (BER) is calculated and displayed in the MATLAB console.

Feel free to experiment with different parameters and adapt the script for your specific OFDM simulation needs.
