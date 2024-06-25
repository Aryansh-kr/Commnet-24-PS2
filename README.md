# Phy-Layer-Design (Quasi 5G NR Communication System)

## Overview

This project aims to design and model a quasi 5G NR (New Radio) system, incorporating essential concepts from 5G that mimic real-world communication systems. The objective is to simulate a communication system that transmits digital data and retrieves it at the receiver despite potential disruptions in the channel. The system includes various blocks such as source, sampling, quantization, source encoding, forward error correction, modulation, pulse shaping, channel effects, and receiver functionalities like synchronization, filtering, and decoding.

## Team Mavericks

* *Aditya Raj*
* *Aryansh Kumar*

## Problem Statement

In this problem statement, we have designed and modeled a quasi 5G NR system, incorporating some important concepts from 5G that mimic real-world communication systems.

## Project Structure

### Transmitter

1. *Source, Sampling, and Quantization*
   - Generate a random digital message.
   - Create floating point values as sampled data.
   - Quantize by taking the floor value.
   
2. *Source Encoder*
   - Convert integers to 2's complement binary numbers.
   - Ensure minimum possible bits needed for communication.
   
3. *Forward Error Correction (FEC)*
   - Introduce redundancy by writing each bit 5 times over to help detect and correct bit errors.
   
4. *Modulation/Mapping*
   - Introduce QAM-64 modulation scheme.
   - Plot the signal constellation.
   
5. *Pulse Shaping*
   - Implement raised cosine filter.
   - Filter the data stream.

### Channel

1. *Rayleigh Fading Channel*
   - Implement a 5-path channel with different delays and path gains.
   
2. *AWGN*
   - Add noise with a specified SNR (6 dB).
   
3. *Timing Offset*
   - Introduce a random timing offset.
   
4. *Frequency Offset (Bonus)*
   - Introduce a random frequency offset.

### Receiver

1. *Carrier Synchronization (Bonus)*
   - Correct the frequency offset using standard MATLAB functions.
   
2. *Timing Synchronization*
   - Correct the timing offset using standard MATLAB functions.
   
3. *Inverse Pulse Shaping*
   - Implement matched filter.
   - Adjust for group delay and filter gain.
   
4. *Channel Equalization (Option 1)*
   - Perform zero-forcing channel equalization.
   
5. *Channel Decoding*
   - Perform inverse repetitive coding.
   
6. *Demodulation/Demapping*
   - Demodulate using QAM demodulation.

## Results

The code calculates the Bit Error Rate (BER) and the number of errors, providing insight into the performance of the quasi 5G NR system.

## Conclusion

This project successfully simulates a quasi 5G NR communication system, incorporating key 5G concepts and demonstrating the robustness of the system against various channel impairments.

## Future Work

* Implement advanced error correction techniques.
* Explore higher-order modulation schemes.
* Optimize the system for real-time performance.

## How to Run

1. Clone the repository.
2. Open the MATLAB script.
3. Run the script to simulate the communication system.
