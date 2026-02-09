# Zipf’s Law of Abbreviation in Bukowski (English–Spanish)

This repository contains the code used to examinate **Zipf’s Law of Abbreviation**
in a poem by Charles Bukowski in English and its Spanish translation.

Zipf’s Law of Abbreviation predicts that more frequent linguistic units tend to be
shorter. The analysis tests this prediction in a short literary text and compares
results across two languages.

---

## Description

The analysis examines the relationship between word frequency and word length using
four methodological variants for each language:

1. Lemmas with stopwords  
2. Lemmas without stopwords  
3. Surface word forms with stopwords  
4. Surface word forms without stopwords  

Linguistic preprocessing is performed with **spaCy**, and the relationship between
frequency and length is evaluated using **Spearman’s rank correlation coefficient**.

---

## Repository contents

- `EXERCISE_1.ipynb`  
  Jupyter notebook containing the full analysis, figures, and results.

- `environment.yml`  
  Conda environment specification with all required dependencies.

- `Bukowski_en_drinking.txt`  
  English poem text (UTF-8 encoded).

- `Bukowski_es_beber.txt`  
  Spanish translation (UTF-8 encoded).


---

## Environment setup

The analysis was conducted in a Conda environment specified in `environment.yml`.

To recreate the environment:

```bash
conda env create -f environment.yml
conda activate spacy_env
