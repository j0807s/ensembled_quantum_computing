# Robust Ensembled Quantum Computing for Variational Quantum Algorithms
**Robust Ensembled Quantum Computing for Variational Quantum Algorithms**\
**_Junsu Kim_**, Suhyun Kim




<p align="center">
<img src="overall_framework.png" width="100%">
</p>

## Abstract
Variational Quantum Algorithms (VQA) are important quantum applications because they can potentially take quantum advantages with Noisy Intermediate-Scale Quantum (NISQ) devices via learnable parameterized quantum gates. However, the error from the noise still degrades the performance of VQA. Furthermore, training VQA using real quantum machines is extremely slow due to the long waiting queue for cloud-based access to IBMQ. In this regard, ensembled quantum computing is one of the key ideas to overcome the aforementioned limitations since it reduces correlated errors while boosting training speed by facilitating currently available devices during training. Unfortunately, the existing ensembled quantum computing framework shows substantial performance variation of VQA depending on each device and its noise level. To tackle these problems, we propose a new framework for VQA that shows consistent performance despite device and noise changes. The framework first selects a primary device, which is more accessible and reliable. Then, it aggressively optimizes a given circuit for the primary device while reducing the number of total SWAP gates for all the given quantum computers. Finally, the framework compensates for the difference in noise levels with random Pauli gates insertion during training and inference.

## Installation

### Prerequisites
* python == 3.8
* ray == 2.2.0
* qiskit == 0.39.4

### Setup
* conda env create -f eqc.yml

## Reproduce observation data
Below commands save the best and the worst VQA circuit architecture based on given quantum devices (default: Lima, Oslo, Manila). Then, start training using multiple devices with the VQA. Finally, save loss function graphs and analyze performance on each device used in training.

## Training
* TBD:
```bash
sh run_vqe.sh
sh run_qml.sh
sh run_qaoa.sh
```
## Results
* Performance on each device: TBD 




