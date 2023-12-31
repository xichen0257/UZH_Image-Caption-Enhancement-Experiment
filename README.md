# Experiment on Enhancing Image Captioning with Entity-Enriched Queries

## Introduction
This repository documents an experiment aimed at enhancing image captioning with entity-enriched queries. The primary objective is to assess whether incorporating named entities within textual queries can improve the accuracy of image captions and retrieval. The study utilizes the SBU Captioned Photo Dataset and measures the impact of entity-enriched queries using the CLIP (Contrastive Language-Image Pretraining) model for text-to-image matching.  
This experiment is conducted as part of the 'Essentials of Text and Speech Processing' course at UZH.

## Data Set
We used the SBU Captioned Photo Dataset, sourced from Flickr. This dataset features image-caption pairs known for their visual relevance, making it ideal for our research.

## Model
We employed the CLIP (Contrastive Language-Image Pretraining) model, specifically the "openai/clip-vit-base-patch32" version.

## Preprocessing
During data preprocessing, non-functional image URLs were removed, and a random subset of 8000 instances was selected.

## Model Training
The model was trained to generate text and image embeddings, both for original titles and NER-enhanced titles.

## Evaluation
We assessed model performance using Precision@K scores. Results indicate that original titles consistently outperformed NER-enhanced titles, possibly due to context length constraints and dataset size limitations. Further optimization is suggested.

## Future Work
Future work could involve exploring the impact of NER types and locations in text, as well as alternative NER entity integration strategies.

## Usage
To reproduce the experiment, follow the instructions in the code provided. Ensure you have the necessary dependencies installed.

## Conclusion
While original titles outperformed NER-enhanced titles in our experiment, the CLIP model demonstrated strong text-to-image matching capabilities.
