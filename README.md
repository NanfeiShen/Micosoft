# CTR Prediction with Transformer | UCLA x Microsoft Ads Capstone

This repository contains code for Click-Through Rate (CTR) prediction using a behavior-enhanced Transformer model. The project was developed as part of the UCLA Master of Data Science in Health Capstone program in collaboration with Microsoft Ads.

## Project Overview

- **Objective**: Improve CTR prediction accuracy by incorporating sequential user behavior data using a Transformer-based deep learning architecture.
- **Data**: Click logs and user profiles from large-scale e-commerce ad interactions (e.g., Taobao dataset).
- **Models**:
  - Baseline: Logistic Regression, LightGBM, MLP
  - Final Model: Transformer with embedding, positional encoding, and attention pooling

## Key Features

- Multi-head self-attention for behavior sequence modeling
- Embedding layers for high-cardinality categorical features
- Handling 30%+ missing data via top-frequency imputation
- Evaluation using AUC and LogLoss metrics

## Results

| Model         | AUC    | LogLoss |
|---------------|--------|---------|
| Logistic Reg. | 0.64   | 0.592   |
| LightGBM      | 0.671  | 0.576   |
| MLP           | 0.675  | 0.571   |
| **Transformer** | **0.687**  | **0.567**   |

## File Structure

- `transformer.ipynb`: Main notebook with data preprocessing, model definition, training, and evaluation.

## Acknowledgements

This project was completed under the guidance of UCLA MDSH faculty and with support from Microsoft Ads.

## License

MIT License (to be added if needed)
