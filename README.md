# Document Re-ranking using Sequence-to-Sequence Model

This project presents a document re-ranking system using a pretrained sequence-to-sequence model (T5). It demonstrates how leveraging the latent knowledge captured during pretraining can improve ranking performance compared to traditional classification-based models like BERT.

## Team Members
- Nishit Munjani (202311026)
- Rohit Rathod (202311039)
- Ayushi Mehta (202311008)
- Pratham Patel (202311022)

## Project Overview
The aim of this project is to investigate whether the T5 model can outperform traditional document ranking methods. We adapt T5 for a generation-based approach to document ranking and evaluate its effectiveness on the MS MARCO dataset.

### Key Features
- **Input**: Query and document pairs, labeled as relevant or not.
- **Model**: Fine-tuned T5 to generate relevance scores.
- **Output**: Documents are re-ranked based on their relevance scores.

## Methodology
1. **Input Sequence**: Query: `q` Document: `d` with a binary label indicating relevance.
2. **Target Generation**: The model outputs “true” or “false” to represent relevance.
3. **Ranking**: Logits are calculated for each document, and softmax is applied to rank documents.
4. **Training**: Fine-tuned on MS MARCO, evaluated on TREC Robust 04 dataset.

## Evaluation Metrics
- NDCG (Normalized Discounted Cumulative Gain)
- MRR (Mean Reciprocal Rank)
- AP (Average Precision)
- Precision



]
