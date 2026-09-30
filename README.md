# Digital Signal Processing Architectures in Verilog

A hardware-oriented DSP project implementing **FIR, FFT, and IIR signal-processing architectures in Verilog**, with MATLAB used for coefficient generation, reference modeling, and output verification.

## Projects

This repository contains three DSP hardware implementations:

1. **FIR Bandpass Filter**
2. **8-Point Radix-2 FFT**
3. **IIR Butterworth Filter — Direct Form II**

---

## 1. FIR Bandpass Filter

### Overview

Implemented a fixed-point FIR bandpass filter in Verilog using coefficients generated from MATLAB.

### Key Features

* Fixed-point **Q2.14** arithmetic
* MATLAB-generated filter coefficients
* Verilog RTL implementation
* Verilog testbench for functional verification
* MATLAB-based output comparison

### Design Flow

```text
MATLAB Filter Design
        ↓
Coefficient Generation
        ↓
Q2.14 Fixed-Point Conversion
        ↓
Verilog FIR Implementation
        ↓
Simulation
        ↓
MATLAB Output Verification
```

---

## 2. 8-Point Radix-2 FFT

### Overview

Designed and implemented an **8-point Radix-2 Fast Fourier Transform (FFT)** architecture in Verilog.

### Key Features

* 8-point Radix-2 FFT
* FSM-based control
* Butterfly processing units
* Complex arithmetic
* Fixed-point signal processing
* MATLAB test-vector verification

### Architecture

```text
Input Samples
     ↓
Bit-Reversal / Data Ordering
     ↓
Stage 1 Butterflies
     ↓
Stage 2 Butterflies
     ↓
Stage 3 Butterflies
     ↓
FFT Output
```

### Verification

MATLAB-generated test vectors were used as reference inputs and outputs to validate the Verilog FFT implementation.

---

## 3. IIR Butterworth Filter

### Overview

Implemented a multi-stage **IIR Butterworth filter using Direct Form II** architecture.

The implementation explores different hardware architectures for improving throughput and understanding hardware resource trade-offs.

### Architectures

Three implementation approa
