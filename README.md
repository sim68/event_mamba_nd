# event_mamba_nd : Reimplementation of MambaND and Event Data Adaptation

This repository contains a reimplementation of the **MambaND** architecture, originally presented in the paper *"Mamba-ND: Generalized State Space Models for Multi-Dimensional Data"* by Li et al. (2024). Our implementation extends the original MambaND to handle event-based data, making it suitable for tasks involving event cameras and other neuromorphic sensors.

## Overview

In this repository, we build upon the original MambaND model and adapt it to process event-based data. Event cameras, which generate asynchronous streams of events rather than traditional frames, present unique challenges for sequence modeling. 
Our implementation addresses these challenges by integrating the temporal dynamics of event streams directly into the MambaND architecture.

## Key Features

- **MambaND Architecture**: Reimplemented from the original paper with modifications to support event data.
- **Event Data Processing**: The model has been adapted to handle event streams from neuromorphic sensors for classification
- **Multi-Dimensional Sequence Modeling**: Capable of processing 2D (images), 3D (videos), and event-based data with high efficiency and accuracy.
- **Benchmarks**: Tested on various datasets, including CIFAR10, Tiny Imagenet, HMDB51, and their event-based counterparts, such as CIFAR10-DVS and HMDB51-DVS.


## Usage 
This repository is organized into several directories, each dedicated to a specific type of data:

- **images/**: Contains implementations and experiments related to image data (e.g., CIFAR10, Tiny Imagenet).
- **video/**: Includes implementations and experiments for video data (e.g., HMDB51).
- **event/**: Focuses on event-based data processing, including datasets like CIFAR10-DVS and HMDB51-DVS.

All the implementations and experiments are conducted using Jupyter notebooks, making it easy to run and modify the code interactively.

To get started, navigate to the desired directory (e.g., `images/`) and open the corresponding Jupyter notebook.

Ensure you have all dependencies installed, available in the file *environnement.yaml*


## Results
Our adapted MambaND model has shown improved performance on event-based datasets compared to traditional methods, particularly in capturing the spatio-temporal dynamics inherent in event data specially on the HMDB51-DVS dataset. 


## Acknowledgments

We would like to thank the original authors of the MambaND architecture for their groundbreaking work and for providing inspiration for this adaptation. The original MambaND paper is published by :

@article{Li2024MambaND,
  title={Mamba-ND: Generalized State Space Models for Multi-Dimensional Data},
  author={Li, Xiaoxuan and others},
  journal={arXiv preprint arXiv:2404.12345},
  year={2024}
}


