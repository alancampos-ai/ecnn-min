# Ecnn mineral

#### Article: <small><strong>Group- and Gauge-Equivariant Convolutional Networks for Binary Segmentation of FeM Mineral Images</strong> <a href=""><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a> <a href=""><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a> <a href="https://drive.google.com/drive/folders/1F9e0RKuGpopX26E9n4Q9zbR6tYKMayiQ?usp=drive_link"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We evaluate group- and gauge-equivariant convolutional networks for binary segmentation and predictive uncertainty reduction in reflected-light mineral images. The gauge-equivariant convolutional network (GECN) combines a typed six-channel input with image-derived local frames and confidence-weighted transport. The analysis characterizes local-frame sensitivity, derives perturbation bounds, and establishes covariance of confidence-weighted transport. Evaluation uses 81 image–mask pairs, five image-wise folds, five optimization seeds, and 25 parameter-matched networks. Within the controlled comparison under direct calibrated inference, GECN increases F1 by 5.44% relative to Plain (PL) and reduces negative log-likelihood (NLL), Brier score, and expected calibration error (ECE) by 29.52%, 27.50%, and 54.00%, respectively. Paired F1 and NLL contrasts against PL are significant under two-sided Wilcoxon tests ($p<10^{-4}$). Runtime, peak GPU memory, floating-point operation counts, and measured energy consumption are also reported.

#### Dependencies

The reference Python version is 3.12.7. External-comparator runs used Python 3.10.19, PyTorch 2.2.0+cu121, and CUDA 12.1. The Docker image uses `pytorch/pytorch:2.4.1-cuda12.4-cudnn9-runtime` with the following dependencies:

* NumPy 1.26.4
* SciPy 1.13.1
* Matplotlib 3.9.2
* Pillow 10.4.0
* NiBabel 5.3.2
* DIPY 1.12.1
* escnn 1.0.11
* PyTorch Geometric 2.6.1
* opt-einsum 3.4.0
* trimesh 4.5.3
* tqdm 4.67.1

#### Installation

```bash
docker build --pull -f docker/Dockerfile -t ecnn-min:latest .
docker run --rm ecnn-min:latest
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
