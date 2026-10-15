# Ecnn mineral

novo link do drive:  https://drive.google.com/drive/folders/1F9e0RKuGpopX26E9n4Q9zbR6tYKMayiQ?usp=drive_link

#### Article:   <small><strong>Equivariant Switching Gain-Graph Descriptor for Mineral Images</strong>  <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a>  <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a>  <a href="https://drive.google.com/drive/folders/1PFo1AklBpse2Tg4RbjPkNxztqyD_DMNY?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We introduce a switching-invariant gain-graph (SIGG) descriptor for paired reflected-light microscopy images and binary mineral masks. SIGG combines canonical multiscale local relations with $D_4$-equivariant component geometry and appearance. Switching reduces local gain profiles from 1,092 to 84 entries and halves padded storage from 36,864 to 18,432. Evaluation uses 81 fields from one iron-ore specimen, 20 query seeds, five source-image folds, and 11,340 transformed partial-view queries per method. Among eleven representations, SIGG achieves mean reciprocal rank (MRR) 0.9874, Recall@1 0.9846, and Recall@5 0.9895. MRR without switching is 0.9877 (Holm-adjusted $p=0.625$). Pooled invariant SIGG attains MRR 0.1111 ($p_{\rm Holm}=5.36\times10^{-14}$). Mean relative equivariance error is $9.12\times10^{-17}$. Paired source-image inference uses Wilcoxon tests, effect sizes, and bootstrap confidence intervals. Sensitivity selection uses outer-training folds. Runtime, memory, energy, and neural floating-point operation counts are reported.

#### Dependencies (evaluation environment)

* Python 3.10.19
* NumPy 1.26.4
* SciPy 1.12.0
* pandas 2.2.3
* scikit-image 0.25.2
* scikit-learn 1.7.2
* PyTorch 2.2.0+cu121
* torchvision 0.17.0
* Matplotlib 3.10.8
* Pillow 11.3.0
* PyYAML 6.0.3
* psutil 7.0.0
* joblib 1.5.3
* pytest 9.1.1

#### Installation

```bash
docker compose -f docker/compose.yaml build
docker compose -f docker/compose.yaml up --abort-on-container-exit
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
