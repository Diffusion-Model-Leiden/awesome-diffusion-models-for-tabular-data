# [Awesome Diffusion Models For Tabular Data](https://arxiv.org/)

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/Diffusion-Model-Leiden/awesome-diffusion-models-for-tabular-data)

We discuss the aspiring studies on diffusion models for tabular data. 

You are very welcomed to read our paper and feel free to leave comments.

[Diffusion Models for Tabular Data: Challenges, Current Progress, and Future Directions (under review)](https://arxiv.org/)

If you found the review paper and this repository helpful, please star this project and cite our survey paper:

```bibtex
@misc{liDiffusion2025,
title = { Diffusion Models for Tabular Data: Challenges, Current Progress, and Future Directions}
author = {Li, Zhong, et al.}
year = {2025},
month = feb,
number = {},
primaryclass = {cs},
doi = {}
}
```

This repository is actively maintained and regularly updated. We highly appreciate valuable recommendations on relevant and interesting research. 

New featured studies will be listed here first.

---
# Table of Contents

- [Awesome Diffusion Models For Tabular Data](#awesome-diffusion-models-for-tabular-data)
- [Table of Contents](#table-of-contents)
- [Timeline of GenAI for Tabular Data](#timeline-of-genai-for-tabular-data)
- [Data Augmentation](#data-augmentation)
  - [Single Table Synthesis](#single-table-synthesis)
  - [Multi-relational Data Synthesis](#multi-relational-data-synthesis)
- [Data Imputation](#data-imputation)
- [Trustworthy Data Synthesis](#trustworthy-data-synthesis)
- [Anomaly Detection](#anomaly-detection)
- [(In Depth) Handling Discrete Data in Diffusion Models](#in-depth-handling-discrete-data-in-diffusion-models)
- [Collection of Datasets](#collection-of-datasets)

# Timeline of GenAI for Tabular Data
![Timeline](materials/TabGenAI2.svg)

# Data Augmentation
```markdown
The topic of data augmentation can be divided into two sub-topics:
  1. Single table synthesis: generation of an entire table or a specific part of a table (over sampling)
  2. Multi-relational data synthesis: generation of multiple tables while considering their intercorrelations and constraints
```
## Single Table Synthesis
|  Abbr.  |   Title  |   Venue & Year |   Code   |   Domain   |
|:--------|:--------:|:--------:|:--------:|:--------:|
SOS | [**Sos: Score-based oversampling for tabular data**](https://arxiv.org/abs/2206.08555) | KDD 2022 | [![Stars](https://img.shields.io/github/stars/jayoungkim408/sos.svg?style=social&label=Star)](https://github.com/jayoungkim408/sos) | Generic|
STaSy | [**STaSy: Score-based Tabular data Synthesis**](https://arxiv.org/abs/2210.04018) | ICLR 2023 | [![Stars](https://img.shields.io/github/stars/JayoungKim408/STaSy.svg?style=social&label=Star)](https://github.com/JayoungKim408/STaSy) | Generic |
TabDDPM | [**Tabddpm: Modelling tabular data with diffusion models**](https://arxiv.org/abs/2209.15421) | ICML 2023 | [![Stars](https://img.shields.io/github/stars/yandex-research/tab-ddpm.svg?style=social&label=Star)](https://github.com/yandex-research/tab-ddpm) | Generic |
CoDi | [**Codi: Co-evolving contrastive diffusion models for mixed-type tabular synthesis**](https://arxiv.org/abs/2304.12654) | ICML 2023 | [![Stars](https://img.shields.io/github/stars/chaejeonglee/codi.svg?style=social&label=Star)](https://github.com/chaejeonglee/codi) | Generic |
MissDiff | [**MissDiff: Training Diffusion Models on Tabular Data with Missing Values**](https://arxiv.org/abs/2307.00467) | ICML Workshop 2023 | N/A | Generic |
AutoDiff | [**AutoDiff: combining Auto-encoder and Diffusion model for tabular data synthesizing**](https://arxiv.org/abs/2310.15479) | NeurIPS Workshop 2023 | [![Stars](https://img.shields.io/github/stars/ucla-trustworthy-ai-lab/autodiffusion.svg?style=social&label=Star)](https://github.com/ucla-trustworthy-ai-lab/autodiffusion) | Generic |
DPM-EHR | [**Synthetic health-related longitudinal data with mixed-type variables generated using diffusion models**](https://arxiv.org/abs/2303.12281) | NeurIPS Workshop 2023 | [Promise to release](https://healthgym.ai/) | Healthcare |
FinDiff | [**Findiff: Diffusion models for financial tabular data generation**](https://arxiv.org/abs/2309.01472) | ICAIF 2023 | [![Stars](https://img.shields.io/github/stars/sattarov/FinDiff.svg?style=social&label=Star)](https://github.com/sattarov/FinDiff) | Finance |
CDTD | [**Continuous Diffusion for Mixed-Type Tabular Data**](https://arxiv.org/abs/2312.10431) | NeurIPS Workshop 2023 | N/A | Generic |
MedDiff | [**MedDiff: Generating electronic health records using accelerated denoising diffusion model**](https://arxiv.org/abs/2302.04355) | ArXiv 2023 | N/A | Healthcare |
EHR-TabDDPM | [**Synthesizing mixed-type electronic health records using diffusion models**](https://arxiv.org/abs/2302.14679) | ArXiv 2023 | N/A | Healthcare |
TabSyn | [**Mixed-Type Tabular Data Synthesis with Score-based Diffusion in Latent Space**](https://arxiv.org/abs/2310.09656) | ICLR 2024 | [![Stars](https://img.shields.io/github/stars/amazon-science/tabsyn.svg?style=social&label=Star)](https://github.com/amazon-science/tabsyn) | Generic |
FlexGen-EHR | [**A Flexible Generative Model for Heterogeneous Tabular EHR with Missing Modality**](https://openreview.net/forum?id=W2tCmRrj7H) | ICLR 2024 | N/A | Healthcare |
EHRDiff | [**EHRDiff: Exploring Realistic EHR Synthesis with Diffusion Models**](https://arxiv.org/abs/2303.05656) | TMLR 2024 | [![Stars](https://img.shields.io/github/stars/sczzz3/ehrdiff.svg?style=social&label=Star)](https://github.com/sczzz3/ehrdiff) | Healthcare |
Forest-Diffusion | [**Generating and imputing tabular data via diffusion and flow-based gradient-boosted trees**](https://arxiv.org/abs/2309.09968) | AISTATS 2024 | [![Stars](https://img.shields.io/github/stars/SamsungSAILMontreal/ForestDiffusion.svg?style=social&label=Star)](https://github.com/SamsungSAILMontreal/ForestDiffusion) | Generic |
TabDiff | [**TabDiff: a Unified Diffusion Model for Multi-Modal Tabular Data Generation**](https://arxiv.org/abs/2410.20626) | NeurIPS Workshop 2024 | [![Stars](https://img.shields.io/github/stars/MinkaiXu/TabDiff.svg?style=social&label=Star)](https://github.com/MinkaiXu/TabDiff) | Generic |
EntTabDiff | [**Entity-based Financial Tabular Data Synthesis with Diffusion Models**](https://doi.org/10.1145/3677052.3698625) | ICAIF 2024 | N/A | Finance |
Imb-FinDiff | [**Imb-FinDiff: Conditional Diffusion Models for Class Imbalance Synthesis of Financial Tabular Data**](https://doi.org/10.1145/3677052.3698659) | ICAIF 2024 | N/A | Finance |
EHR-D3PM | [**Guided discrete diffusion for electronic health record generation**](https://arxiv.org/abs/2404.12314) | ArXiv 2024 | N/A | Healthcare |
TabUnite | [**TabUnite: Efficient Encoding Schemes for Flow and Diffusion Tabular Generative Models**](https://openreview.net/forum?id=Zoli4UAQVZ) | OpenReview 2024 | [![Stars](https://img.shields.io/github/stars/jacobyhsi/TabUnite.svg?style=social&label=Star)](https://github.com/jacobyhsi/TabUnite) | Generic |
FraudDiffuse | [**FraudDiffuse: Diffusion-aided Synthetic Fraud Augmentation for Improved Fraud Detection**](https://doi.org/10.1145/3677052.3698658) | ICAIF 2024 | N/A | Finance |
FraudDDPM | [**Synthetic Data Generation for Fraud Detection Using Diffusion Models**](https://doi.org/10.11610/isij.5534) | ISIJ 2024 | N/A | Finance |

## Multi-relational Data Synthesis
|  Abbr.  |   Title  |   Venue & Year  |   Code   |   Domain   |
|:--------|:--------:|:--------:|:--------:|:--------:|
ClavaDDPM | [**ClavaDDPM: Multi-relational Data Synthesis with Cluster-guided Diffusion Models**](https://arxiv.org/abs/2405.17724) | NeurIPS 2024 | [![Stars](https://img.shields.io/github/stars/weipang142857/clavaddpm.svg?style=social&label=Star)](https://github.com/weipang142857/clavaddpm) | Generic |
GNN-TabSyn | [**Relational Data Generation with Graph Neural Networks and Latent Diffusion Models**](https://openreview.net/forum?id=MNLR2NYN2Z#discussion) | NeurIPS Workshop 2024 | [![Stars](https://img.shields.io/github/stars/ValterH/relational-graph-conditioned-diffusion.svg?style=social&label=Star)](https://github.com/ValterH/relational-graph-conditioned-diffusion) | Generic |

# Data Imputation
```markdown
Data imputation involves generating plausible values to fill in missing entries in tabular data
```
|  Abbr.  |   Title  |   Venue & Year  |   Code   |   Domain   |
|:--------|:--------:|:--------:|:--------:|:--------:|
TabCSDI | [**Diffusion models for missing value imputation in tabular data**](https://arxiv.org/abs/2210.17128) | NeurIPS Workshop 2022 | [![Stars](https://img.shields.io/github/stars/pfnet-research/CSDI_T.svg?style=social&label=Star)](https://github.com/pfnet-research/CSDI_T) | Generic |
TabDiff | [**TabDiff: a Unified Diffusion Model for Multi-Modal Tabular Data Generation**](https://arxiv.org/abs/2410.20626) | NeurIPS Workshop 2024 |  [![Stars](https://img.shields.io/github/stars/MinkaiXu/TabDiff.svg?style=social&label=Star)](https://github.com/MinkaiXu/TabDiff)| Generic |
SimpDM | [**Self-supervision improves diffusion models for tabular data imputation**](https://arxiv.org/abs/2407.18013) | CIKM 2024 | [![Stars](https://img.shields.io/github/stars/yixinliu233/simpdm.svg?style=social&label=Star)](https://github.com/yixinliu233/simpdm) | Generic |
MTabGen | [**Diffusion models for tabular data imputation and synthetic data generation**](https://arxiv.org/abs/2407.02549) | ArXiv 2024 | Promise to release upon acceptance| Generic |
DDPM-Perlin | [**Natural generative noise diffusion model imputation**](https://doi.org/10.1016/j.knosys.2024.112310) | KBS 2024 | [Empty repository](https://github.com/arizbw/perlin-diffusion-imputation) | Generic |
NewImp | [**Rethinking the diffusion models for missing data imputation: A gradient flow perspective**](https://proceedings.neurips.cc/paper_files/paper/2024/hash/cb1ba6a42814bf83974ed45ffdb72efa-Abstract-Conference.html) | NeurIPS 2024 | [![Stars](https://img.shields.io/github/stars/JustusvLiebig/NewImp.svg?style=social&label=Star)](https://github.com/JustusvLiebig/NewImp) | Generic |
DiffPuter | [**Unleashing the Potential of Diffusion Models for Incomplete Data Imputation**](https://arxiv.org/abs/2405.20690) | OpenReview 2024 | [![Stars](https://img.shields.io/github/stars/hengruizhang98/DiffPuter.svg?style=social&label=Star)](https://github.com/hengruizhang98/DiffPuter) | Generic |
TabSyn | [**Mixed-Type Tabular Data Synthesis with Score-based Diffusion in Latent Space**](https://arxiv.org/abs/2310.09656) | ICLR 2024 | [![Stars](https://img.shields.io/github/stars/amazon-science/tabsyn.svg?style=social&label=Star)](https://github.com/amazon-science/tabsyn) | Generic |
Forest-Diffusion | [**Generating and imputing tabular data via diffusion and flow-based gradient-boosted trees**](https://arxiv.org/abs/2309.09968) | AISTATS 2024 | [![Stars](https://img.shields.io/github/stars/SamsungSAILMontreal/ForestDiffusion.svg?style=social&label=Star)](https://github.com/SamsungSAILMontreal/ForestDiffusion) | Generic |

# Trustworthy Data Synthesis
```markdown
Trustworthy data synthesis aims to generate realistic surrogate values for sensitive entries while keeping the overall utility of the tabular data.
```
|  Abbr.  |   Title  |   Venue & Year  |   Code   |   Domain   |
|:--------|:--------:|:--------:|:--------:|:--------:|
SiloFuse | [**SiloFuse: Cross-silo Synthetic Data Generation with Latent Tabular Diffusion Models**](https://arxiv.org/abs/2404.03299) | ICDE 2024 | N/A | Generic |
FedTabDiff | [**FedTabDiff: Federated Learning of Diffusion Probabilistic Models for Synthetic Mixed-Type Tabular Data Generation**](https://arxiv.org/abs/2401.06263) | ArXiv 2024 | [![Stars](https://img.shields.io/github/stars/sattarov/fedtabdiff.svg?style=social&label=Star)](https://github.com/sattarov/fedtabdiff) | Generic |
FairTabDDPM | [**Balanced Mixed-Type Tabular Data Synthesis with Diffusion Models**](https://arxiv.org/abs/2404.08254) | ArXiv 2024 | [![Stars](https://img.shields.io/github/stars/comp-well-org/fair-tab-diffusion.svg?style=social&label=Star)](https://github.com/comp-well-org/fair-tab-diffusion) | Generic |
DP-Fed-FinDiff | [**Differentially Private Federated Learning of Diffusion Models for Synthetic Tabular Data Generation**](https://arxiv.org/abs/2412.16083) | ArXiv 2024 | N/A | Finance |

# Anomaly Detection
```markdown
In anomaly detecion, diffusion models are used to learn the “normal” distribution of data from the known set and identify anomalies as deviations from this learned distribution in the unseen data.
```
|  Abbr.  |   Title  |   Venue & Year  |   Code   |   Domain   |
|:--------|:--------:|:--------:|:--------:|:--------:|
TabADM | [**TabADM: Unsupervised Tabular Anomaly Detection with Diffusion Models**](https://arxiv.org/abs/2307.12336) | ArXiv 2023 | N/A | Generic |
DTE | [**On Diffusion Modeling for Anomaly Detection**](https://arxiv.org/abs/2305.18593) | ICLR 2024 | [![Stars](https://img.shields.io/github/stars/vicliv/DTE.svg?style=social&label=Star)](https://github.com/vicliv/DTE) | Generic |
SDAD | [**Self-supervised enhanced denoising diffusion for anomaly detection**](https://doi.org/10.1016/j.ins.2024.120612) | Inf. Sci. 2024 | [Under construction](https://github.com/lsmiao1209/DOD_codes) | Generic |
NSCBAD | [**Anomaly Detection by Estimating Gradients of the Tabular Data Distribution**](https://openreview.net/forum?id=7QDIFrtAsB) | OpenReview 2024 | [Supplementary Material](https://openreview.net/forum?id=7QDIFrtAsB) | Generic |
FraudDiffuse | [**FraudDiffuse: Diffusion-aided Synthetic Fraud Augmentation for Improved Fraud Detection**](https://doi.org/10.1145/3677052.3698658) | ICAIF 2024 | N/A | Finance |
FraudDDPM | [**Synthetic Data Generation for Fraud Detection Using Diffusion Models**](https://doi.org/10.11610/isij.5534) | ISIJ 2024 | N/A | Finance |

# (In Depth) Handling Discrete Data in Diffusion Models
To be finished

# Collection of Datasets
