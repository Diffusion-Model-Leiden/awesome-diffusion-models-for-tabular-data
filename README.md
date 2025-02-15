# [Awesome Diffusion Models For Tabular Data](https://arxiv.org/)

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
## Table of Contents

- [Awesome Diffusion Models For Tabular Data](#awesome-diffusion-models-for-tabular-data)
  - [Table of Contents](#table-of-contents)
- [Data Augmentation](#data-augmentation)
  - [Single Table Synthesis](#single-table-synthesis)
  - [Multi-relational Data Synthesis](#multi-relational-data-synthesis)
- [Data Imputation](#data-imputation)
- [Trustworthy Data Synthesis](#trustworthy-data-synthesis)
- [Anomaly Detection](#anomaly-detection)
- [(In Depth) Handling Discrete Data in Diffusion Models](#in-depth-handling-discrete-data-in-diffusion-models)


# Data Augmentation

## Single Table Synthesis
- Sos: Score-based oversampling for tabular data, KDD 2022, [[Paper](https://arxiv.org/abs/2206.08555)], [Official [Codes](https://github.com/jayoungkim408/sos)]
- STaSy: Score-based Tabular data Synthesis, ICLR 2023, [[Paper](https://arxiv.org/abs/2210.04018)], [Official [Codes](https://github.com/JayoungKim408/STaSy)]
- Tabddpm: Modelling tabular data with diffusion models, ICML 2023, [[Paper](https://arxiv.org/abs/2209.15421)], [Official [Codes](https://github.com/yandex-research/tab-ddpm)]
- Codi: Co-evolving contrastive diffusion models for mixed-type tabular synthesis, ICML 2023, [[Paper](https://arxiv.org/abs/2304.12654)], [Official [Codes](https://github.com/chaejeonglee/codi)]
- MissDiff: Training Diffusion Models on Tabular Data with Missing Values, ICML Workshop 2023, [[Paper](https://arxiv.org/abs/2307.00467)]
- AutoDiff: combining Auto-encoder and Diffusion model for tabular data synthesizing, NeurIPS Workshop 2023, [[Paper](https://arxiv.org/abs/2310.15479)], [Official [Codes](https://github.com/ucla-trustworthy-ai-lab/autodiffusion)]
- Synthetic health-related longitudinal data with mixed-type variables generated using diffusion models, NeurIPS Workshop 2023, [[Paper](https://arxiv.org/abs/2303.12281)], [[Promise to release codes](https://healthgym.ai/)]
- Findiff: Diffusion models for financial tabular data generation, ICAIF 2023, [[Paper](https://arxiv.org/abs/2309.01472)], [Official [Codes](https://github.com/sattarov/FinDiff)]
- Continuous Diffusion for Mixed-Type Tabular Data, NeurIPS Workshop 2023, [[Paper](https://arxiv.org/abs/2312.10431)]
- MedDiff: Generating electronic health records using accelerated denoising diffusion model, ArXiv 2023, [[Paper](https://arxiv.org/abs/2302.04355)]
- Synthesizing mixed-type electronic health records using diffusion models, ArXiv 2023, [[Paper](https://arxiv.org/abs/2302.14679)]
- Mixed-Type Tabular Data Synthesis with Score-based Diffusion in Latent Space, ICLR 2024, [[Paper](https://arxiv.org/abs/2310.09656)], [Official [Codes](https://github.com/amazon-science/tabsyn)]
- A Flexible Generative Model for Heterogeneous Tabular EHR with Missing Modality, ICLR 2024
- EHRDiff: Exploring Realistic EHR Synthesis with Diffusion Models, TMLR 2024, [[Paper](https://arxiv.org/abs/2303.05656)], [Official [Codes](https://github.com/sczzz3/ehrdiff)]
- Generating and imputing tabular data via diffusion and flow-based gradient-boosted trees, AISTATS 2024, [[Paper](https://arxiv.org/abs/2309.09968)], [Official [Codes](https://github.com/SamsungSAILMontreal/ForestDiffusion)]
- TabDiff: a Unified Diffusion Model for Multi-Modal Tabular Data Generation, NeurIPS Workshop 2024, [[Paper](https://arxiv.org/abs/2410.20626)], [Official [Codes](https://github.com/MinkaiXu/TabDiff)]
- Entity-based Financial Tabular Data Synthesis with Diffusion Models, ICAIF 2024, [[Paper](https://doi.org/10.1145/3677052.3698625)]
- Imb-FinDiff: Conditional Diffusion Models for Class Imbalance Synthesis of Financial Tabular Data, ICAIF 2024, [[Paper](https://doi.org/10.1145/3677052.3698659)]
- Guided discrete diffusion for electronic health record generation, ArXiv 2024, [[Paper](https://arxiv.org/abs/2404.12314)]
- TabUnite: Efficient Encoding Schemes for Flow and Diffusion Tabular Generative Models, OpenReview 2024
- FraudDiffuse: Diffusion-aided Synthetic Fraud Augmentation for Improved Fraud Detection, ICAIF 2024, [[Paper](https://doi.org/10.1145/3677052.3698658)]
- Synthetic Data Generation for Fraud Detection Using Diffusion Models, ISIJ 2024, [[Paper](https://doi.org/10.11610/isij.5534)]

## Multi-relational Data Synthesis
- ClavaDDPM: Multi-relational Data Synthesis with Cluster-guided Diffusion Models, NeurIPS 2024, [[Paper](https://arxiv.org/abs/2405.17724)], [Official [Codes](https://github.com/weipang142857/clavaddpm)]
- Relational Data Generation with Graph Neural Networks and Latent Diffusion Models, NeurIPS Workshop 2024, [[Paper](https://openreview.net/forum?id=MNLR2NYN2Z#discussion)], [Official [Codes](https://github.com/ValterH/relational-graph-conditioned-diffusion)]

# Data Imputation
- Diffusion models for missing value imputation in tabular data, NeurIPS Workshop 2022, [[Paper](https://arxiv.org/abs/2210.17128)], [Official [Codes](https://github.com/pfnet-research/CSDI_T)]
- TabDiff: a Unified Diffusion Model for Multi-Modal Tabular Data Generation, NeurIPS Workshop 2024, [[Paper](https://arxiv.org/abs/2410.20626)]
- Self-supervision improves diffusion models for tabular data imputation, CIKM 2024, [[Paper](https://arxiv.org/abs/2407.18013)], [Official [Codes](https://github.com/yixinliu233/simpdm)]
- Diffusion models for tabular data imputation and synthetic data generation, ArXiv 2024, [[Paper](https://arxiv.org/abs/2407.02549)], [Promise to release codes upon acceptance]
- Natural generative noise diffusion model imputation, KBS 2024, [[Paper](https://doi.org/10.1016/j.knosys.2024.112310)], [[Empty repostory](https://github.com/arizbw/perlin-diffusion-imputation)]
- Rethinking the diffusion models for missing data imputation: A gradient flow perspective, NeurIPS 2024, [Official [Codes]((https://github.com/JustusvLiebig/NewImp))]
- Unleashing the Potential of Diffusion Models for Incomplete Data Imputation, OpenReview 2024, [[Paper](https://arxiv.org/abs/2405.20690)], [Official [Codes](https://github.com/hengruizhang98/DiffPuter)]
- Mixed-Type Tabular Data Synthesis with Score-based Diffusion in Latent Space, ICLR 2024, [[Paper](https://arxiv.org/abs/2310.09656)], [Official [Codes](https://github.com/amazon-science/tabsyn)]
- Generating and imputing tabular data via diffusion and flow-based gradient-boosted trees, AISTATS 2024, [[Paper](https://arxiv.org/abs/2309.09968)], [Official [Codes](https://github.com/SamsungSAILMontreal/ForestDiffusion)]
  
# Trustworthy Data Synthesis
- SiloFuse: Cross-silo Synthetic Data Generation with Latent Tabular Diffusion Models, ICDE 2024, [[Paper](https://arxiv.org/abs/2404.03299)]
- FedTabDiff: Federated Learning of Diffusion Probabilistic Models for Synthetic Mixed-Type Tabular Data Generation, ArXiv 2024, [[Paper](https://arxiv.org/abs/2401.06263)], [Official [Codes](https://github.com/sattarov/fedtabdiff)]
- Balanced Mixed-Type Tabular Data Synthesis with Diffusion Models, ArXiv 2024, [[Paper](https://arxiv.org/abs/2404.08254)], [Official [Codes](https://github.com/comp-well-org/fair-tab-diffusion)]
- Differentially Private Federated Learning of Diffusion Models for Synthetic Tabular Data Generation, ArXiv 2024, [[Paper](https://arxiv.org/abs/2412.16083)]

# Anomaly Detection
- TabADM: Unsupervised Tabular Anomaly Detection with Diffusion Models, ArXiv 2023, [[Paper](https://arxiv.org/abs/2307.12336)]
- On Diffusion Modeling for Anomaly Detection, ICLR 2024, [[Paper](https://arxiv.org/abs/2305.18593)], [Official [Codes](https://github.com/vicliv/DTE)]
- Self-supervised enhanced denoising diffusion for anomaly detection, Inf. Sci. 2024, [[Paper](https://doi.org/10.1016/j.ins.2024.120612)], [Official [Codes under construction](https://github.com/lsmiao1209/DOD_codes)]
- Anomaly Detection by Estimating Gradients of the Tabular Data Distribution, OpenReview 2024, [[Paper](https://openreview.net/forum?id=7QDIFrtAsB)], [Official [Codes in Supplementary Material](https://openreview.net/forum?id=7QDIFrtAsB)]
- FraudDiffuse: Diffusion-aided Synthetic Fraud Augmentation for Improved Fraud Detection, ICAIF 2024, [[Paper](https://doi.org/10.1145/3677052.3698658)]
- Synthetic Data Generation for Fraud Detection Using Diffusion Models, ISIJ 2024, [[Paper](https://doi.org/10.11610/isij.5534)]

# (In Depth) Handling Discrete Data in Diffusion Models
To be finished