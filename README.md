# Skincare Review Analytics on Dot and Key Moisturizers (SMA Project)

End-to-end Social Media Analytics project by **Divya Bothra** focused on scraping, cleaning, and analyzing online skincare product (moisturizer) reviews using Python and NLP. [web:1]

---

## Overview

This project implements a complete pipeline for skincare review analytics: collecting raw reviews from the web, preprocessing text, extracting entities and parts of speech, and generating word and topic summaries for moisturizers. [web:1]  
The outputs can be used for marketing analysis, product insight generation, and as input to further models on customer opinions. [web:1]

---

## Features

- Web scraping of moisturizer reviews from selected online sources. [web:1]  
- Text cleaning, tokenization, and normalization of review text. [web:1]  
- Part-of-speech (POS) tagging and Named Entity Recognition (NER) on reviews. [web:1]  
- Word frequency analysis and topic-style summaries at product level. [web:1]  
- Export of intermediate and final datasets to Excel for easy reuse and reporting. [web:1]

---

## Repository Structure

- `Web_Scraping.ipynb`  
  Scrapes moisturizer reviews and builds the core dataset (`SMA_Dataset.xlsx` and related files). [web:1]

- `SMA_Capstone_DivyaBothra -2.ipynb`  
  Main analysis notebook for cleaning, NLP processing, POS/NER, and topic/word summaries. [web:1]

- `Scraped Datasets/`  
  Raw scraped review data. [web:1]

- `cleaned_reviews.xlsx`  
  Reviews after cleaning and preprocessing. [web:1]

- `cleaned_with_tokens.xlsx`  
  Token-level representation of cleaned reviews. [web:1]

- `Word Frequency Excels/`  
  Word and token frequency outputs for each product or group. [web:1]

- `NER + POS Tagging Files/`  
  Outputs from NER and POS tagging pipelines. [web:1]

- `topic_summary_by_moisturizer.xlsx`  
  Topic and keyword summaries aggregated at the moisturizer level. [web:1]

---

## Tech Stack

- Python  
- Jupyter Notebook  
- Excel (for exporting and sharing outputs) [web:1]

---

## Getting Started

1. Clone this repository:  
