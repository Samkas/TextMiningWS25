# Text Mining - Lesson 1 Notebooks

This folder contains four comprehensive Jupyter notebooks covering essential text mining and natural language processing techniques. The course uses real-world datasets to teach practical NLP implementations.

## Datasets

All notebooks work with two datasets:

### **AG News** (English)
- 120,000 training samples + 7,600 test samples
- 4 balanced news categories: World, Sports, Business, Sci/Tech
- Source: [Kaggle - AG News Classification Dataset](https://www.kaggle.com/datasets/amananandrai/ag-news-classification-dataset)

### **10kGNAD** (German)
- German news articles across 9 different categories
- Source: [Kaggle - 10kGNAD](https://www.kaggle.com/datasets/mexwell/10kgnad)

---

## Notebook Overview

### 1. **spaCy_WS25.ipynb**
Industrial-strength NLP with spaCy for production applications.

**Topics Covered:**
- Loading AG News and 10kGNAD datasets
- Data exploration and visualization
- spaCy pipelines and models
- Named Entity Recognition (NER)
- Dependency parsing
- Lemmatization and tokenization
- Language-specific processing

**Key Concepts:**
- spaCy's efficient pipeline architecture
- Practical applications in production
- Multilingual NLP support
- Fast and memory-efficient processing

---

### 2. **nltk_gensim_WS25.ipynb**
Introduction to NLTK and Gensim libraries for NLP tasks.

**Topics Covered:**
- Data loading from both English (AG News) and German (10kGNAD) datasets
- NLTK library overview:
  - 50+ built-in corpora and lexical resources
  - WordNet integration
  - Tokenization and linguistic processing
- Gensim library for:
  - Word embeddings
  - Topic modeling
  - Document similarity
- Multilingual NLP support

**Key Concepts:**
- NLTK as a comprehensive NLP toolkit
- Working with linguistic resources
- Topic modeling and semantic representations
- Handling multilingual text data

---

### 3. **Features_Clustering_WS25.ipynb**
Feature extraction, representation, and text clustering techniques.

**Topics Covered:**
- Data loading and sampling (5,000 documents)
- Text cleaning with regex patterns
- Feature representation:
  - **CountVectorizer**: Bag-of-words approach
  - **TfidfVectorizer**: TF-IDF weighting with scikit-learn
- NLTK stopwords integration
- Accent normalization (unicode handling)
- Clustering algorithms for document organization

**Key Concepts:**
- Text preprocessing and cleaning
- Feature engineering for text data
- Comparison of different vectorization methods
- Dimensionality reduction for clustering

---

### 4. **classification_WS25.ipynb**
Text classification using word count representations and machine learning.

**Topics Covered:**
- Data loading and sampling for computational efficiency
- Train/test split (65/35) - best practices for avoiding data leakage
- Word count matrix creation using CountVectorizer
- Feature transformation: TF-IDF vectorization
- Text classification with machine learning models
- Confusion matrix and accuracy evaluation

**Key Concepts:**
- Importance of splitting data BEFORE any transformations
- Training vs. test set handling
- Multiclass classification

---

## Dataset Structure

Each dataset is loaded with the following structure:

**AG News:**
- `Label`: Category ID (1-4)
- `Title`: Article headline
- `Article`: Full article text
- `features`: Title + Article combined

**10kGNAD:**
- `Label`: Category name
- `Article`: Full article text

---

## Prerequisites

### Required Libraries
```
pandas
numpy
scikit-learn
nltk
gensim
spacy
matplotlib
tqdm
```

### Dataset Location
Ensure the data files are located in:
```
../data/AGNews/train.csv
../data/AGNews/test.csv
../data/10kGNAD/train.csv
../data/10kGNAD/test.csv
```

---
