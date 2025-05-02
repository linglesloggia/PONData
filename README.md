# Citation

If you use this dataset in your research, please cite our paper:

```bibtex```

# Dynamic PON Configuration Dataset

This repository contains an open dataset collected from our experimental study on dynamic configuration of Passive Optical Networks (PON). The dataset captures detailed measurements under varying traffic conditions and T-CONT configurations.

## Dataset Overview

The dataset includes measurements from a commercial GPON platform equipped with SDN orchestration to enable traffic-adaptive uplink resource allocation. It serves as a valuable resource for analyzing GPON performance and testing dynamic configuration strategies in realistic network conditions.

## Download the Dataset
The dataset is available for download [here](https://partage.imt.fr/index.php/s/nEGj4ENnWYgFGE2)

### Contents
- 2.43 GB of CSV data
- Includes traffic generator outputs and network parameters
- Currently 6 datasets are available (still growing), each with different configurations and traffic patterns
- Network configurations and user traffic profiles recorded at regular 12-minute intervals across the emulated 24-hour period.
- Performance results for each combination of configuration and traffic profile, including eighty-eight metrics per direction (uplink and downlink) such as latency, frame loss ratio, bit error rate, throughput, and packet size.
- Traffic patterns derived from both real-world studies and synthetic scenarios, applied to various network configurations.
- Data stored in multi-indexed Pandas DataFrames for structured analysis.


## Experimental Setup

![Diagram](imgs/infrastructure_photograph.png)
The datasets were carried out using commercial deployment equipment, including:
- OLT
- 16 ONUs
- Traffic generator
- Ethernet switches
- Server
- SDN controller

### Traffic Patterns
-  Real-world traffic patterns derived from studies [1,2,3] on residential and business networks

## Use Cases

This dataset can be used for:
1. Analyzing GPON performance under diverse traffic conditions
2. Training ML models for network configuration prediction
3. Testing dynamic bandwidth allocation algorithms
4. Benchmarking PON solutions in research
5. Studying QoS management in shared optical infrastructure

### References
[1] Feknous et al., *Internet traffic analysis*, 2014.  
[2] Zhang et al., *Residential traffic modeling*, 2010.  
[3] Kihl et al., *Traffic characterization for IPTV*, 2010.  
