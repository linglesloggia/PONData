# Fixed-Mobile Convergence (FMC) PON Dataset

This repository contains an open dataset collected from our experimental study on Dynamic PON Configuration for Fixed-Mobile Convergence applications.

## Dataset Overview

The dataset contains measurements from a commercial GPON platform with SDN orchestration for dynamic T-CONT configuration, enabling traffic-adaptive uplink resource allocation. It demonstrates how existing GPON FTTH infrastructure can efficiently support small cell backhaul in FMC scenarios.

## Download the Dataset
The dataset is available for download from the following mirrors:

[French mirror](https://partage.imt.fr/index.php/s/R8mBAHFo5gL7Wym)

[Uruguayan mirror](https://nube.fing.edu.uy/index.php/s/LdDn25qaCitWY6Z)

### Contents
- 44,385 measurement points (703.8 MB of CSV data)
- Collected over a two-week period
- Includes traffic generator outputs and network parameters

## Experimental Setup

The experiment used commercial deployment devices including:
- OLT
- 16 ONUs (1 for mobile traffic, 15 for fixed clients)
- Traffic generator
- Switches
- Server
- SDN controller layer

### Traffic Patterns
- **Fixed users**: 15 ONUs with profiles showing minimal usage at 3 a.m. and peak usage at 9 p.m.
- **Mobile traffic**: 1 dedicated ONU with peak traffic at 3 p.m.
- Users classified into heavy, medium, and low usage groups

### T-CONT Configuration
- **TCONT 1** for mobile traffic (defined by FIR parameter)
- **TCONT 3** for fixed clients (defined by PIR and CIR parameters)
- Multiple FIR-PIR combinations tested throughout data collection

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
1. Analyzing PON behavior under various traffic conditions
2. Training prediction models for network configuration optimization
3. Developing algorithms for dynamic resource allocation
4. Benchmarking FMC solutions
5. Research on QoS management in shared optical infrastructure

## Citation

If you use this dataset in your research, please cite our paper:

```bibtex
 
```

## License

This dataset is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.

## Acknowledgements

This work was funded by the DGE IPCEI ME/CT Orange and the STIC-AmSud RAMONaaS projects and was conducted in the framework of the Lab'Optic, a joint research initiative between the UMR-6285 Lab-STICC, the UMR 6082 Foton Institute and Orange Innovation.

