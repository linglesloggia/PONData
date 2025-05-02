## License & Citation

This dataset is made available under the **Open Data Commons Attribution-NonCommercial 1.0 License (ODC-BY-NC 1.0)**.

You are free to use this dataset for non-commercial research and academic purposes **as long as you give appropriate credit**.

### 📌 Citation Requirement

If you use this dataset in a publication, please cite it as follows:

```bibtex
@misc{TO_BE_UPDATED,
  author = {L.Inglés, L.Anet Neto, C.Rattaro, M.Morvan, A.Castro, L.Nuaymi},
  title = {PON Physical Twin: Enabling Third-party Research on FTTH Optimization with Open Datasets},
  year = {},
  howpublished = {},
  note = {DOI or publication details to be added}
}
```
# Dynamic PON Configuration Dataset

This repository contains an open dataset collected from our experimental study on dynamic configuration of Passive Optical Networks (PON). The dataset captures detailed measurements under varying traffic conditions and T-CONT configurations.

## Dataset Overview


The dataset is available for download [here](https://partage.imt.fr/index.php/s/nEGj4ENnWYgFGE2)

The dataset includes:

- 2.43 GB of CSV data
- Includes traffic generator outputs and network parameters
- Currently 6 datasets are available (still growing), each with different configurations and traffic patterns
- Network configurations and user traffic profiles recorded at regular 12-minute intervals across the emulated 24-hour period.
- Performance results for each combination of configuration and traffic profile, including eighty-eight metrics per direction (uplink and downlink) such as latency, frame loss ratio, bit error rate, throughput, and packet size.
- Traffic patterns derived from both real-world studies [1,2,3] and synthetic scenarios, applied to various network configurations.
- Data stored in multi-indexed Pandas DataFrames for structured analysis.


## Experimental Setup

![Diagram](imgs/infrastructure_photograph.png)

The dataset was collected in a controlled laboratory environment, simulating a GPON network with the following components:

- OLT (Optical Line Terminal)
- 16 ONUs (Optical Network Units)
- Traffic generator
- Ethernet switches
- Server
- SDN controller

## Use Cases

This dataset can be used for:
1. Analyzing GPON performance under diverse traffic conditions
2. Training ML models for network configuration prediction
3. Testing dynamic bandwidth allocation algorithms
4. Benchmarking PON solutions in research
5. Studying QoS management in shared optical infrastructure

Thank you for your interest in our dataset! We hope it serves as a valuable resource for your research and development efforts in the field of PON optimization and network performance analysis. This dataset is continuously growing. New configurations and measurements will be added over time.


### References
[1] Feknous et al., *Internet traffic analysis*, 2014.  
[2] Zhang et al., *Residential traffic modeling*, 2010.  
[3] Kihl et al., *Traffic characterization for IPTV*, 2010.  
