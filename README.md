# Transformers on Genome Sequences


<img src="./dnabert_umap.png" width="400" height="400">

This repository demonstrates the use of transformers, including pre-trained BERT and DNABERT, to analyze and visualize genome sequences. The project downloads mitochondrial DNA sequences from various organisms, preprocesses them, and uses these transformer models to generate embeddings. These embeddings are then visualized using UMAP and clustered to observe the relationships between sequences from different organisms.

## Table of Contents

1. [Overview](#overview)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Notebook Sections](#notebook-sections)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

## Overview

This project aims to provide insights into the heterogeneity and relationships between genome sequences from different organisms. By leveraging transformer models like pre-trained BERT and DNABERT, we can generate meaningful embeddings that capture the underlying structure of the sequences. The embeddings are visualized using UMAP and clustered to reveal patterns and relationships.

## Installation

To get started, clone the repository and install the required libraries:

```bash
git clone https://github.com/galenwilkerson/Transformers-on-Genome-Sequences.git
cd Transformers-on-Genome-Sequences
pip install -r requirements.txt
```

## Usage

1. **Download the DNA sequences**:
   The script automatically downloads mitochondrial DNA sequences for human, mouse, rat, and zebrafish from Ensembl.

2. **Run the Jupyter Notebook**:
   Open and run the Jupyter Notebook to process the DNA sequences, generate embeddings using pre-trained BERT and DNABERT, and visualize them using UMAP.

```bash
jupyter notebook "Transformers on Genome Sequences.ipynb"
```

## Notebook Sections

1. **Introduction**:
   Overview of the project and objectives.

2. **Setup**:
   Importing libraries, defining URLs for DNA sequences, and functions for downloading and decompressing datasets.

3. **Data Download**:
   Downloading mitochondrial DNA sequences from Ensembl for various organisms.

4. **BERT Embeddings**:
   Using pre-trained BERT to generate embeddings for the DNA sequences.

5. **DNABERT Embeddings**:
   Using DNABERT to generate embeddings for the DNA sequences.

6. **Dimensionality Reduction**:
   Applying UMAP to reduce the dimensionality of the embeddings for visualization.

7. **Clustering**:
   Performing clustering on the UMAP-reduced embeddings using Gaussian Mixture Models.

8. **Visualization**:
   Visualizing the UMAP projections with cluster labels and organism labels.

## Results

The UMAP visualization shows clusters of DNA sequence embeddings, colored by the organism they belong to. The project highlights the relationships and differences between the sequences from different organisms.

![UMAP projection](path/to/your/image/umap_plot_with_organisms.png)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
