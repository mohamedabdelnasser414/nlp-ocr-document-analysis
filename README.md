# Intelligent Document Processing System

An end-to-end document analysis pipeline that combines Optical Character Recognition (OCR), Computer Vision, and Natural Language Processing (NLP) techniques to extract, analyse, and classify information from digital documents.

The project uses OpenCV, Tesseract OCR, spaCy, and TF-IDF to process image-based and text-based documents, detect document features, extract text, identify entities, and generate meaningful insights from unstructured data.

---

## Project Overview

This project demonstrates how OCR, Computer Vision, and NLP can be integrated into a single workflow to automate document understanding.

The system is capable of:

- Extracting text from images and PDF documents
- Preprocessing documents to improve OCR accuracy
- Detecting document regions and visual features
- Performing text cleaning and normalization
- Tokenising and lemmatising extracted text
- Removing stop words and irrelevant content
- Identifying named entities using spaCy
- Extracting keywords using TF-IDF
- Categorising and analysing document content

---

## Technologies Used

### Computer Vision
- OpenCV
- NumPy
- Matplotlib

### OCR
- Tesseract OCR
- PyTesseract

### Natural Language Processing
- spaCy
- NLTK
- Regular Expressions (Regex)

### Data Processing
- Pandas
- Scikit-learn

---

## Workflow

### 1. Document Input

The system accepts:

- PDF documents
- Scanned images
- JPEG images
- PNG images

---

### 2. OCR Preprocessing

Several image enhancement techniques are applied before OCR:

- Grayscale conversion
- Noise reduction
- Binary thresholding
- Adaptive thresholding
- Image segmentation
- Contour detection

These preprocessing steps improve OCR performance on scanned and low-quality documents.

---

### 3. Text Extraction

Text is extracted using Tesseract OCR.

The system can:

- Extract complete document text
- Detect individual words
- Generate OCR bounding boxes
- Visualise detected text regions

---

### 4. NLP Processing

Extracted text undergoes several NLP preprocessing stages:

#### Tokenisation
Splits text into individual words and tokens.

#### Stop Word Removal
Removes common words that provide little analytical value.

#### Lemmatisation
Converts words into their base dictionary form.

Example:

```text
running → run
cars → car
better → good
```

#### Named Entity Recognition (NER)

Identifies entities such as:

- Person names
- Organisations
- Locations
- Dates
- Monetary values

---

### 5. Keyword Extraction

TF-IDF is used to identify the most important terms within each document.

This helps highlight:

- Key topics
- Frequently discussed concepts
- Document-specific terminology

---

### 6. Feature Detection

Computer Vision techniques are used to identify visual document components such as:

- Text regions
- Logos
- Shapes
- Advertisements
- Image areas

---

## Example Pipeline

```text
Document
    ↓
Preprocessing
    ↓
OCR Extraction
    ↓
Text Cleaning
    ↓
Tokenisation
    ↓
Lemmatisation
    ↓
NER
    ↓
TF-IDF
    ↓
Document Insights
```

---

## Project Structure

```text
.
├── data/
│   ├── images/
│   ├── pdfs/
│   └── outputs/
│
├── notebooks/
│   ├── OCR_Preprocessing.ipynb
│   ├── NLP_Processing.ipynb
│   ├── Feature_Detection.ipynb
│   └── Document_Analysis.ipynb
│
├── results/
│   ├── extracted_text/
│   ├── visualisations/
│   └── keyword_reports/
│
├── requirements.txt
└── README.md
```

---

## Sample Results

### OCR

- Successfully extracted text from scanned images and PDF documents
- Generated word-level OCR bounding boxes
- Improved OCR accuracy through image preprocessing

### NLP

- Extracted named entities from documents
- Generated document keywords using TF-IDF
- Normalised text through tokenisation and lemmatisation

### Computer Vision

- Detected document features and regions
- Applied contour-based segmentation
- Visualised document layouts

---

## Learning Outcomes

This project demonstrates practical applications of:

- Optical Character Recognition (OCR)
- Computer Vision
- Natural Language Processing (NLP)
- Document Understanding
- Information Extraction
- Feature Detection
- Text Mining
- Machine Learning Preprocessing

---

## Future Improvements

Potential enhancements include:

- Deep learning-based document classification
- Table extraction from invoices and forms
- Layout-aware document understanding
- Transformer-based NLP models
- Automatic document categorisation
- Invoice field extraction and validation

---

## Author

Mohamed Abdelnasser

MSc Big Data Analytics & Artificial Intelligence  
Atlantic Technological University (ATU)
