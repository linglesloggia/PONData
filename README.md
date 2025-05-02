# Dynamic PON Configuration Dataset

This repository contains an open dataset collected from our experimental study on dynamic configuration of Passive Optical Networks (PON). The dataset captures detailed measurements under varying traffic conditions and T-CONT configurations.

## Dataset Overview

The dataset includes measurements from a commercial GPON platform equipped with SDN orchestration to enable traffic-adaptive uplink resource allocation. It serves as a valuable resource for analyzing GPON performance and testing dynamic configuration strategies in realistic network conditions.

## Download the Dataset
The dataset is available for download from the following mirrors:

- [French mirror](https://partage.imt.fr/index.php/s/R8mBAHFo5gL7Wym)  
- [Uruguayan mirror](https://nube.fing.edu.uy/index.php/s/LdDn25qaCitWY6Z)

### Contents
- 44,385 measurement points (703.8 MB of CSV data)
- Collected over a two-week period
- Includes traffic generator outputs and network parameters

## Experimental Setup

The experiment was carried out using commercial deployment equipment, including:
- OLT
- 16 ONUs
- Traffic generator
- Ethernet switches
- Server
- SDN controller

### Traffic Patterns
- **Fixed clients**: 15 ONUs with usage profiles showing minimal activity at 3 a.m. and peak at 9 p.m.
- **High-demand ONU**: 1 ONU simulating bursty or mobile-like traffic, with peak usage at 3 p.m.
- Users were grouped into heavy, medium, and low usage categories

### T-CONT Configuration
- **TCONT 1**: Used for high-demand traffic, defined by the FIR parameter
- **TCONT 3**: Used for regular client traffic, defined by PIR and CIR parameters
- Multiple combinations of FIR, PIR, and CIR values were tested during data collection

## Dataset Structure

```
├── README.md
├── data/
│   ├── raw/           # Raw CSV data from measurements
│   └── processed/     # Cleaned and processed data
├── metadata/          # Information about data structure and collection
└── models/            # Prediction models from the paper
```


## Use Cases

This dataset can be used for:
1. Analyzing GPON performance under diverse traffic conditions
2. Training ML models for network configuration prediction
3. Testing dynamic bandwidth allocation algorithms
4. Benchmarking PON solutions in research
5. Studying QoS management in shared optical infrastructure

## Citation

If you use this dataset in your research, please cite our paper:

```bibtex
 
