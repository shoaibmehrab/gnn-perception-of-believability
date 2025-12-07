## Enhancing GNN-based Fake News Detection with User Believability

This repository contains the source code and implementation for the research on improving Graph Neural Network (GNN) performance for fake news detection by incorporating user believability scores. This work is directly related to the findings for Research Question 2 (RQ2) in our paper accepted in ACM CSCW 2025 and published in Proceedings of the ACM on Human-Computer Interaction.

**Paper:** [Understanding News Consumers’ Perceptions of Believability: A Study of Real and Fake News](https://dl.acm.org/doi/pdf/10.1145/3757691)

## Project Overview

The core idea of this research is to investigate whether integrating user believability as a feature can enhance the performance of GNN models in distinguishing between real and fake news. This repository provides the code to reproduce the experiments and results discussed in our paper.

We have implemented and evaluated three different GNN architectures:
*   **Graph Convolutional Network (GCN)**
*   **Graph Attention Network (GAT)**
*   **GraphSAGE**

The code demonstrates how to build, train, and evaluate these models on a news propagation graph, using node features that include user believability scores.

## Repository Structure

The repository is organized as follows:

*   `src/`: Contains the Jupyter notebooks with the implementations of the GNN models.
    *   `GCN.ipynb`, `GAT.ipynb`, `SAGE.ipynb`: Base implementations for the GNN models.
    *   `GCN_human_evaluation.ipynb`, `GAT_human_evaluation.ipynb`, `SAGE_human_evaluation.ipynb`: Notebooks for evaluating the models with features derived from human believability scores.
*   `datasets/`: This directory should contain the processed dataset files (`node_attributes.npy`, `adjacency_matrix.npy`, `labels_v2.npy`) used in the notebooks.
*   `saved-models/`: This directory is used to store the trained model weights.

## Getting Started

### Prerequisites

The models are implemented using PyTorch and PyTorch Geometric. You can install the required dependencies using a package manager like `pip`.

### Usage

1.  Place the required dataset files in the `datasets/` directory.
2.  Open the Jupyter notebooks in the `src/` directory to see the implementation details for each model.
3.  Run the cells in the notebooks to train and evaluate the models. The `*_human_evaluation.ipynb` files are particularly relevant to the core research question.

## Citation

If you use this code or our findings in your research, please cite our paper:

```bibtex
@article{sakib2025understanding,
  title={Understanding News Consumers' Perceptions of Believability: A Study of Real and Fake News},
  author={Sakib, Mostofa Najmus and Ahmed, Md Shoaib and Spezzano, Francesca and Hamby, Anne},
  journal={Proceedings of the ACM on Human-Computer Interaction},
  volume={9},
  number={7},
  pages={1--31},
  year={2025},
  publisher={ACM New York, NY, USA}
}

```
