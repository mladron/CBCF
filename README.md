# CBCF
Configurable Bucket Cuckoo Filter (CBCF)

## Description
The goal of CBCF is to reduce the False Positive Rate of Cuckoo filters operating below full capacity. This code is used in the paper "Cuckoo Filters and Bloom Filters: Comparison and Application to Packet Classification" by P. Reviriego, J. Martínez, D. Larrabeiti and S. Pontarelli

## Compilation
This Visual Studio C++ project consists of 3 files: CF.hpp (declaration file), CF.cpp (source file) and main.cpp (test bench)

## Command line arguments
Command line arguments are:
- m: filter mode, default value is 1 for cbcf, 0 is for standard cf
- s: filter size, default value is 8192
- o: filter occupancy, default value is 95%
- r: runs (trials), default value is 10000
- b: scrubbing, default value is 1
- i: scrub iterations, default value is 20
- f: fingerprint_bits, default value is f = {12, 15, 18}

**example: cbcf.exe i=30 r=5000 f=12**

## License
MIT
