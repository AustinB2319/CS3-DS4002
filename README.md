# CS3 – DS 4002

This repository contains all materials needed to complete the Letterboxd Sentiment Analysis case study for DS 4002.

---

## Repository Contents

**CS3 - Hook Document.pdf**
Start here. This one-page document introduces the case study, provides context for the problem, and describes your mission as a data scientist.

**CS3 - Rubric.pdf**
Read this after the hook. It outlines the full requirements for your deliverable, including expected code structure, data organization, evaluation criteria, and reflection guidelines.

---

## DATA Folder

**LetterboxdTop250-5000reviews.csv**
The raw dataset containing user reviews and star ratings from Letterboxd's Top 250 films. This is your primary data source. If you need to re-download it, the original can be found on Kaggle at:
https://www.kaggle.com/datasets/alarchemn/letterbox-top250-short-reviews

---

## MATERIALS Folder

### Context Articles

| File | Description |
|------|-------------|
| *How is Letterboxd Reshaping Film Culture?* | Background on the platform and its user base |
| *Sarcasm or Praise? The Art of Sentiment Analysis with Deep Learning in Film Reviews* | Motivation for applying sentiment analysis to film review text |
| *Getting Started with Sentiment Analysis using Python* | Accessible introduction to sentiment analysis concepts and tools |
| *Exploring Hugging Face: Sentiment Analysis* | Practical guide to using HuggingFace transformer models |
| *CardiffNLP Twitter-RoBERTa-Base Sentiment* | Model card for a recommended pretrained sentiment model |

**Example Results.png**
A sample output showing what your feature-level accuracy analysis might look like when complete

--- 

## A Note on Engineered Features

The rubric asks you to engineer and analyze four text features. Here is a brief explanation of each:

**Review Length**
The total number of characters or words in a review. Longer reviews may contain more nuanced or mixed sentiment that is harder for a model to classify correctly.

**Emoji Count**
The number of emoji characters present in a review. Emojis are a common way users express emotion informally and may signal sentiment that the model was not trained to interpret.

**Capitalization Ratio**
The proportion of alphabetic characters in a review that are uppercase (e.g. a review that is ALL CAPS has a high capitalization ratio). High capitalization often signals strong emotion, sarcasm, or emphasis, which can confuse a model trained on more neutral text.

**Language**
The detected language of the review text. The recommended pretrained model was trained primarily on English-language data, so reviews written in other languages may be predicted less accurately.
