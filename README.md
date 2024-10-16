# 🚀 SVD-based Recommendation System

## Overview

This project implements a recommendation system using the Singular Value Decomposition (SVD) algorithm to predict user preferences based on implicit feedback. Designed for scenarios like music streaming or e-commerce, this system leverages user interactions (e.g., song plays) to recommend items without the need for explicit ratings.

## Table of Contents

- [Problem Statement](#problem-statement)
- [Solution](#solution)
- [Key Insights](#key-insights)
- [Results](#results)
- [Usage](#usage)
- [Requirements](#requirements)
- [Installation](#installation)
- [License](#license)

## Problem Statement

The dataset used in this project lacks direct ratings, which is a common challenge in recommendation systems. The goal is to recommend items based on implicit feedback derived from user behavior, such as the frequency of song plays or product views.

## Solution

To tackle this problem, the SVD algorithm from the Surprise library in Python was utilized. SVD is effective for factorizing user-item interaction matrices and predicting missing values based on implicit feedback.

### Key Steps:

1. **Data Preparation**: Transform user interactions into a User-Item Matrix, where interactions are represented as implicit ratings.
2. **Matrix Factorization**: Apply SVD to decompose the matrix into latent factors representing user preferences and item attributes.
3. **Prediction**: Generate predicted scores for unseen items, allowing for personalized recommendations.

## Key Insights

- SVD is robust in scenarios where explicit ratings are not available, leveraging implicit signals effectively.
- Evaluation metrics such as Root Mean Square Error (RMSE) and Mean Absolute Error (MAE) demonstrated the model's accuracy:
  - RMSE: ~0.4558
  - MAE: ~0.4149
- This approach can be adapted to various domains, including music, e-commerce, and video streaming services.

## Results

The SVD model significantly reduced the error margin, establishing a strong foundation for personalized recommendations based on user interactions.

## Usage

To explore the code and implementation, check out the GitHub repository. Feel free to clone the project and experiment with the code.

## Requirements

- Python 3.x
- Surprise library
- NumPy
- Pandas

## Installation

```bash
# Clone the repository
git clone https://github.com/assia-briere/music_Recommendation_System.git

# Change into the project directory
cd svd-recommendation-system

# Install the required packages
pip install -r requirements.txt
```

## License

[MIT License](LICENSE)
