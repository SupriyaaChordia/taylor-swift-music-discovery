# Taylor Swift: Music Discovery & Lyric Analysis

Exploring a historical snapshot of Taylor Swift’s music through audio features, song recommendations, lyric search, and keyword analysis.

**[Explore the notebook](Taylor_Swift_Music_Discovery_and_Lyric_Analysis.ipynb)**

## Overview

This project combines exploratory data analysis with tools for music discovery and lyric exploration. It uses Spotify-derived audio features and lyric data to examine catalog patterns, find similar songs, locate phrases, and identify distinctive words.

| Component | Approach |
| --- | --- |
| Audio-feature analysis | Visualize release patterns, popularity, musical mode, and relationships among audio features |
| Song recommendations | Rank tracks by Euclidean distance across selected audio features |
| Lyric search | Match phrases across songs without distinguishing capitalization and display surrounding lines |
| Keyword analysis | Calculate TF-IDF scores for songs on *Lover* and explore lyric word frequencies through word clouds |

## Methods and limitations

The recommender compares content features rather than listener histories. Its default feature set uses seven measures on a 0–1 scale; custom combinations may require additional scaling or weighting. Similarity scores are not evidence of listener preference, and no held-out recommendation evaluation or user experiment is reported.

Popularity scores describe the dataset snapshot, rather than current Spotify rankings. Lyric matching and occurrence counts require further checks for punctuation and overlapping context. The word-cloud display uses lyric word frequencies, separately from the TF-IDF keyword rankings.

## Tools

Python, BabyPandas, NumPy, Matplotlib, IPython, ipywidgets, WordCloud, and Pillow.

## Viewing and running

Open the linked notebook to inspect the code and saved outputs. Interactive widgets require a running Jupyter environment.

To rerun the notebook, install the listed Python packages and provide the original files at these relative paths:

- `data/lyrics.csv`
- `data/tswift.csv`
- `data/albums.csv`
- `data/billions_club.csv`
- `data/word_counts.csv`
- `data/images/heart.jpeg`

The portfolio copy preserves outputs from the completed notebook and removes assignment instructions and grading cells. It has not been rerun after editing. The original data and image asset must be added separately if they are not already included in this repository.

## Team and attribution

Completed by **Supriyaa Chordia and Siya Jatia** as a **UC San Diego DSC 10 course project (2024)**. The coursework supplied the assignment scaffold and some interface/display helpers; the notebook retains that attribution and the original project references. This repository presents a cleaned portfolio copy of the team’s work.

Data sources referenced in the original project include the Spotify and Genius APIs. Additional inspiration and source credits are listed in the notebook.
