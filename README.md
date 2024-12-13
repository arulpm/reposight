# Project Overview

This repository contains the code and resources for a scientific paper search application that leverages embedding models and LLMs to enhance search capabilities and interactivity. The application allows users to search academic papers, summarize content, and query methods using a user-friendly mobile interface.

## Features

- **Data Preprocessing**: Prepares academic datasets for embedding generation.
- **Triplet Generation**: Creates triplets for model training, ensuring relevance.
- **Fine-Tuning**: Fine-tunes the embedding model for domain-specific searches.
- **Vector Store Management**: Handles the storage and retrieval of vector embeddings for fast and accurate searches.

## Directory Structure

```
.
├── finetune.ipynb        # Notebook for fine-tuning embedding models
├── Generate_Triplet.ipynb # Notebook for generating triplets for training
├── praproses_data.ipynb   # Notebook for preprocessing datasets
├── Vector_store.ipynb     # Notebook for vector store operations
└── README.md             # Documentation (this file)
```

## Notebooks Overview

### 1. `finetune.ipynb`
- Fine-tunes the GTE base embedding model using domain-specific data.
- Utilizes triplets generated to improve embedding relevance.
- Implements TensorFlow workflows for efficient training on GPUs.

### 2. `Generate_Triplet.ipynb`
- Generates triplets (anchor, positive, negative samples) for training.
- Ensures high-quality triplets to optimize model learning.
- Outputs datasets ready for fine-tuning.

### 3. `praproses_data.ipynb`
- Handles preprocessing tasks such as cleaning, tokenization, and normalization.
- Prepares data for embedding generation and triplet creation.

### 4. `Vector_store.ipynb`
- Manages vector embedding storage and retrieval.
- Interfaces with Google Cloud Storage for efficient data handling.
- Provides methods for similarity searches and nearest-neighbor queries.

## Technology Stack

- **Backend**: Python with FastAPI
- **Embeddings**: GTE base (v1.5) in TensorFlow

## How to Contribute

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit changes: `git commit -m 'Add feature'`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Contributors and collaborators
- Resources and libraries used
- Special thanks to academic institutions for dataset contributions

