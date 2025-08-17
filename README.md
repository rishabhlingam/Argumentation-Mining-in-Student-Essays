# Thesis Code Repository  

This repository contains the code developed for my Master’s thesis:  
**“A Study on Sentence-Level Argument Identification in Imbalanced Student Essay Corpora”**  
*Florida Atlantic University, 2025*  

---

## Project Overview  

This project investigates how **transformer-based models (BERT and its variants)** can identify argumentative components in **student essays at the sentence level**.  

Essays were annotated using categories from the **Writing Across the Curriculum (WAC) assessment rubric**, but the dataset was **highly imbalanced** (dominant “Normal Text” vs. rare categories like “Thesis” or “Organizational Framework”).  

To address these challenges, several approaches were implemented:  

- **Baseline Model** – Fine-tuned BERT for flat sentence classification.  
- **Context-Aided Models** – Pairing each sentence with surrounding text to incorporate discourse context.  
- **Syntactic Feature Models** – Augmenting BERT with **part-of-speech (POS)** tags via:  
  - Appended POS tags  
  - Replaced POS tags  
  - POS embeddings  
- **Distribution-Aware Hierarchical Model** – Breaking classification into levels based on label distribution to improve minority-class detection.  

Additional contributions include:  

- **Data preprocessing** (sentence segmentation, cleaning, annotation alignment)  
- **Annotation consistency checks** using *Cohen’s Kappa*  
- **Evaluation scripts** for precision, recall, and F1-scores  

---

## Dataset  

- Essays were collected and annotated through FAU’s **Writing Across the Curriculum (WAC) program** (College Writing 1 & 2).  
- Due to privacy and licensing restrictions, **raw essays are not included** in this repository.  

---

## Repository Notes  

- The code reflects **exploratory and iterative development** during thesis research.  
- Scripts are **not organized sequentially** for direct execution.  
- Refer to the thesis PDF (included in the repository) for:  
  - Methodology  
  - Experimental flow  
  - Model configurations  
  - Results and analysis  

---

