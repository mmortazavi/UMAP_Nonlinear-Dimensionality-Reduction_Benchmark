# UMAP_Nonlinear-Dimensionality-Reduction_Benchmark
A primer to Uniform Manifold Approximation and Projection (UMAP)
developed by Leland McInnes, Git: https://github.com/lmcinnes/umap, Paper: https://arxiv.org/abs/1802.03426

Objective: I aim to compare the newly developed UMAP for Nonlinear Dimensionality Reduction. In order to do that I am using various dataset to compare UMAP mainly with t-SNE. For the first two examples (Swiss Roll Data, Severed Sphere) others comonly used dimensionality reductions methods are given for comparisons purposes. Let's get started.

The content:

- Swiss Roll Data
- Severed Sphere
- Handwritten Digits
- Half-Moon Data
- Concentric Circles

First let's quickly look at the abstract of the UMAP paper:

UMAP (Uniform Manifold Approximation and Projection) is a novel manifold learning technique for dimension reduction. UMAP is constructed from a theoretical framework based in Riemannian geometry and algebraic topology. The result is a practical scalable algorithm that applies to real world data. The UMAP algorithm is competitive with t-SNE for visualization quality, and arguably preserves more of the global structure with superior run time performance. Furthermore, UMAP as described has no computational restrictions on embedding dimension, making it viable as a general purpose dimension reduction technique for machine learning.

Advantageous over e.g. t-SNE:
UMAP is fast. It can handle large datasets and high dimensional data (beyond what t-SNE packages can).

UMAP isn't just for visualisation! You can use UMAP as a general purpose dimension reduction technique as a preliminary step to other machine learning tasks. It partners well with the hdbscan clustering.

UMAP often performs better at preserving aspects of global structure of the data than t-SNE (better "big picture")

UMAP supports a wide variety of distance functions, including non-metric distance functions such as cosine distance and correlation distance. You can finally embed word vectors properly using cosine distance!

UMAP has solid theoretical foundations in manifold learning. This both justifies the approach and allows for further extensions that will soon be added to the library (embedding dataframes, semi-supervised dimension reduction, etc.).

*disclaimer: I have borrowed code snippets from Scikit-learn, and a bit from Sebastian Raschka blog (https://sebastianraschka.com/)
