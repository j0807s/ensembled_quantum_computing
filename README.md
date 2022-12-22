# ensembled quantum computing (ISCA'22)

* This repository includes all the scripts for reproducing the observation data of the robust eqc project ([link](https://j0807s.github.io/projects/2_project/)).

## Installation

### Prerequisites
* python == 3.8
* ray == 2.2.0
* qiskit == 0.39.4

### Setup
* conda env create -f eqc.yml

## Reproduce observation data
* Used machines for observation: Quito, Manila, Lima, Oslo, Nairobi, Belem

```bash
python main.py
```

## Results
* All the test loss values depending on devices : ob_loss.txt
* Number of accesses on each device during training : ob_accesses.txt




