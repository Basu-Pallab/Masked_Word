# Masked_Word
Project for the course : Computational Understanding of  Meaning 
# BERT Gap Expectation After ACCUSATIVE Wh-Word

This project investigates whether BERT models anticipate a syntactic gap at the linearly available position after encountering an **ACCUSATIVE case-marked question word** in the matrix clause.

## 🧪 Research Question

> Does BERT expect a syntactic gap in the linearly available position after encountering an accusative-marked WH-word?

## 📁 Project Structure

project/
├── dataset/
│ └── input_mask.csv # Dataset with masked inputs for BERT
├── MODEL-1.py # Model script to generate top-5 predictions at [MASK]
├── MODEL-2.py
├── MODEL-3.py
├── Files_from_Model_output/ # Output files from the three models
├── clean_model_output.py # Script to clean and extract top 5 tokens and probabilities
├── analysis.R # R code for statistical analysis
└── README.md


## 🧭 Workflow

1. **Input Preparation**  
   The `dataset/input_mask.csv` contains masked sentences for model evaluation.

2. **Prediction with BERT**  
   Run `MODEL-1.py`, `MODEL-2.py`, and `MODEL-3.py` to obtain the **top-5 predictions** at the `[MASK]` position.  
   The results are saved in the `Files_from_Model_output/` directory.

3. **Cleaning and Extraction**  
   Use `clean_model_output.py` to extract the **top-5 tokens** and their corresponding **probabilities** from each model's output.

4. **Analysis**  
   The cleaned data is analyzed using R (`analysis.R`) to determine BERT’s expectations about syntactic gaps.

## 💡 Dependencies

### Python:
- `transformers`
- `torch`
- `pandas`

### R:
- `tidyverse`
- `lme4`
- `lmerTest`

## 📜 License

This project is for academic research purposes.

