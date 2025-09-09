# Music Genre Classification 🎵

Classify music genres using machine learning! This project uses logistic regression to predict one of 10 genres from the GTZAN dataset with 69% accuracy.

## Dataset
- **GTZAN Music Genre Dataset:** 1,000 songs (100 per genre)
- **Genres:** Blues, Classical, Country, Disco, Hip-hop, Jazz, Metal, Pop, Reggae, Rock
- **Features:** MFCCs, Spectral Centroid, ZCR

## Results
- **Accuracy:** 69% (6.9x better than random!)
- **Best Performers:** Jazz, Classical, Metal (85% each)
- **Trickiest:** Country, Reggae (50% each) - mixed genres

## Key Insights
- Hyperparameter tuning confirmed the model was already well-optimized
- Mixed-origin genres (Country, Reggae) are harder to classify
- Audio features successfully capture genre-distinguishing patterns

## Quick Start
```bash
git clone https://github.com/anisharamesh21/MusicClassifier.git
cd MusicClassifier
pip install pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook model_training.ipynb
```

To reproduce results: Open model_training.ipynb or hyperparameter_tuning.ipynb

Note: This project uses pre-extracted features (features.txt). To extract features from scratch, follow these steps:<br>
- Download the [GTZAN Dataset](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification) <br>
- Run features_extracter.ipynb to generate your own features<br>
- Or use the provided features.txt to skip feature extraction

## Files
- features_extractor.ipynb - Extraction of major features from audios
- eda.ipynb - Exploratory Data Analysis
- model_training.ipynb - Model Training using Logistic Regression
- hyperparameter_tuning.py - GridSearchCV optimization
- features.txt - GTZAN audio features

## Tech Stack
Python | scikit-learn | pandas | seaborn | matplotlib

*Built during summer 2025 while learning ML!* 🚀
