# Nasa Space Apps Challenge 2025 Hackathan
# A World Away: Hunting for Exoplanets with AI

## Overview

This project dataset uses the observations made by "NASA Kepler Space Telescope" and downloaded using "Kepler labelled time-series dataset on Kaggle" to detect exoplanets using their light curves. I started with a CNN model and switch to a MLP model due to time restrictions to mitigate the ipmact of complexness of CNN model. Finally, I deploy the trained model into a simple web app. 

## Dataset
- **Source**: [NASA Kepler Mission](https://www.nasa.gov/mission_pages/kepler/main/index.html)  
- **Kaggle**: [Kaggle – Exoplanet Hunting in Deep Space](https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data)

## Project Structure
- `exo_planet_hunt.ipynb` → Training pipeline (CNN + MLP, visualizations)
- `web_app.ipynb` → Gradio web app demo
- `requirements.txt` → Dependencies

## Results
- MLP with oversampling to mitigate the heavily imbalance nature if dataset.
- Visualization includes confusion matrices and predicted light curves.

## Web App
Interactive demo using Gradio:
- Paste light curve flux comma separated values
- Model predicts whether a planet exists
- Plots the input curve with probabilities

## Credits
- Dataset: NASA Kepler Mission (via Kaggle)
- Code inspiration: PyTorch community tutorials + Kaggle kernels + Gradio documentation
