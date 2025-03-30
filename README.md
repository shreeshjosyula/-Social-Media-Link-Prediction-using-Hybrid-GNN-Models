# Hybrid GNN for Social Media Link Prediction

## Overview
This project presents a **Hybrid Graph Neural Network (GNN)** model for link prediction in social media networks. It combines the strengths of **Graph Convolutional Networks (GCN), Graph Attention Networks (GAT), and Message Passing Neural Networks (MPNN)** to achieve **enhanced predictive performance**.

## Features
- **Hybrid GNN Model**: Integrates GCN, GAT, and MPNN.
- **Link Prediction**: Predicts potential relationships in social media networks.
- **Graph Processing**: Leverages **PyTorch Geometric (PyG)**.
- **Performance Evaluation**: Assesses accuracy, precision, recall, F1-score, and AUC-ROC.

## Installation
Ensure you have **Python 3.8+** and install the dependencies:

```bash
pip install torch torchvision torchaudio torch-geometric numpy pandas matplotlib
```

## Dataset
The project utilizes publicly available social media datasets. Preprocessing includes:
- **Data Cleaning**: Removing missing/incomplete records.
- **Feature Engineering**: Extracting node embeddings.
- **Graph Construction**: Building edge relationships.

## Model Architecture
The hybrid model follows this layered approach:
1. **GCN Layer** – Captures graph structure.
2. **GAT Layer** – Applies attention-based weighting.
3. **MPNN Layer** – Enhances message-passing across nodes.
4. **Fully Connected Layers** – Aggregates information for final predictions.

## Training
Run the training script with:
```bash
python train.py
```
- Uses **Adam optimizer** with L2 regularization.
- Supports **batch training** and **graph sampling**.

## Evaluation
The model is evaluated using:
- **Accuracy**
- **Precision/Recall/F1-score**
- **ROC-AUC Curve**
- **Comparative Analysis with Standalone GNNs**

## Results
Key findings from our experiments:
- **GCN Accuracy:** 83.44%
- **GAT Accuracy:** 82.25%
- **MPNN Accuracy:** 74.12%
- Hybrid Model **outperforms standalone GNNs** in link prediction tasks.

## Future Work
- Real-time dynamic graph adaptation.
- Scalability improvements.
- Multi-faceted link prediction (strength/type of relationships).

## Contributors
- **Sai Shreesh Josyula** - [Wilfrid Laurier University](mailto:josy3880@mylaurier.ca)
- **Vaibhav Kaushal** - [Wilfrid Laurier University](mailto:kaus0160@mylaurier.ca)

## Citation
If you use this project, please cite:
```
@article{HybridGNN2025,
  author = {Josyula, S. S. and Kaushal, V.},
  title = {Social Media and Link Prediction Analysis Using GNN Models},
  year = {2024}
}
```

## License
This project is licensed under the **MIT License**.
