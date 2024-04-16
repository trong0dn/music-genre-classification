# music-genre-classification

---
> **Preamble:** This notebook was adapted from an Introduction to Machine Learning course assignment. This notebook is intended to demonstrate a basic understanding of classification models and exploration of concepts in machine learning.
---

> **Goal:** To develop music genre detection machine learning model using audio files (potentially) in real time.

> **Objective:**: Using the GTZAN dataset to create a classifier that can classify what the music genre is playing! 🎷🎸🎹🎺
Develop a ‘baseline solution’ that uses a pretrained classifier and fine-tuned it on the musical genre classification task using transfer learning.

> **Instructions:** The entire full notebook should run in approximately 120 minutes to run on T4 GPU. The solutions for this notebook are self-contained. This notebook was intended to be executed and tested on Google Colab. Using the commands: `runtime → run all`.

> **Dataset:** GTZAN Dataset.

Download from source: https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification?resource=download

Placed under `My Drive` in Google Drive directory and renamed as `GTZAN Genre Collection.zip`

Music. Experts have been trying for a long time to understand sound and what differenciates one song from another. How to visualize sound. What makes a tone different from another. This data hopefully can give the opportunity to do just that.

- *genres original* - A collection of 10 genres with 100 audio files each, all having a length of 30 seconds (the famous GTZAN dataset, the MNIST of sounds)
- *images original* - A visual representation for each audio file. One way to classify data is through neural networks. Because NNs (like CNN, what we will be using today) usually take in some sort of image representation, the audio files were converted to Mel Spectrograms to make this possible.
- *2 CSV files* - Containing features of the audio files. One file has for each song (30 seconds long) a mean and variance computed over multiple features that can be extracted from an audio file. The other file has the same structure, but the songs were split before into 3 seconds audio files (this way increasing 10 times the amount of data we fuel into our classification models). With data, more is always better.

> **Runtime Tips:** Select `Runtime -> Change Runtime Type` under `Hardware accelerator` click on `CPU` or `T4 GPU`.
