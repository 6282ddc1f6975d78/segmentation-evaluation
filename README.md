# Toward Interpretable Evaluation Measures for Time Series Segmentation
This repository contains code to reproduce the papers results

Disclaimer: this is a temporary repository for anonymous submission. If accepted, we will provide a detailed and structured open source repository.

## Library Dependencies
To run our code, we recommand using a Python 3.9.18 virtual environment using the following dependencies.
More details are provided in the archive.
```bash
pip install -r requirements.txt
```
## Dataset Preparation
You can download the datasets used in the paper from the following links:


| Dataset   | Type               | Download Link |
|----------|----------|--------------------|
| MoCap   | Real-world | [download](https://drive.google.com/file/d/1Z3HRSxUUfjiPRMzGrOcGie63S1HXA8nf/view?usp=sharing) |
| ActRecTut| Real-world | [download](https://drive.google.com/file/d/1tU5EmxRUk37TzgvpkcgTMQSVG8DBGCUt/view?usp=sharing) |
| PAMAP2| Real-world | [download](https://drive.google.com/file/d/11zwi7PwJiRujncT7kt0NOGOo_GavSSo2/view?usp=sharing) |
| UscHad| Real-world | [download](https://drive.google.com/file/d/1kBHPZZCCN1zrZd7CoSGzG3_W0Jdsm9kF/view?usp=sharing) |
| UcrSeg| Real-world | [download](https://drive.google.com/file/d/1nGH-l3tkp18SauzUUR6P0FhlhEQDLTu2/view?usp=sharing) |

After downloading the datasets, move them to the '\data' directory, ensuring the following directory structure:

```
.
├── data
│   ├── ActRecTut
│   │   ├── subject1_walk
│   │   │   ├── S111.dat
│   │   │   ├── ...
│   │   ├── subject2_walk
│   │   │   ├── S111.dat
│   │   │   ├── ...
│   ├── MoCap
│   │   ├── 4d
│   │   │   ├── amc_86_01.4d
│   │   │   ├── ...
│   │   ├── raw
│   │   │   ├── amc_86_01.txt
│   │   │   ├── ...
│   ├── PAMAP2
│   │   ├── Protocol
│   │   │   ├── subject101.dat
│   │   │   ├── ...
│   ├── USC-HAD
│   │   ├── Subject1
│   │   ├── Subject2
│   │   ├── ...
│   ├── UCRSEG
│   │   ├── Cane_100_2345.txt
│   │   ├── DutchFactory_24_2184.txt
│   │   ├── ...

```
## Experiments command

Simply execute the experiments.py and evaluation.py scripts located in the root folder.

## Acknowledgements

This work leverages the [E2USd](https://github.com/AI4CTS/E2Usd/tree/main/Baselines) implementation as its foundation.

Our gratitude extends to the authors of the following studies for making their datasets publicly available:
- [UCRSEG](https://doi.org/10.1109/ICDM.2017.21)
- [MoCap](https://dl.acm.org/doi/abs/10.1145/2588555.2588556)
- [ActRecTut](https://dl.acm.org/doi/abs/10.1145/2499621)
- [PAMAP2](https://doi.org/10.1109/ISWC.2012.13)
- [USCHAD](https://doi.org/10.1145/2370216.2370438)
