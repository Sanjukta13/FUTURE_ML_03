# AI Resume Screening and Candidate Ranking System

## Project Overview

Recruiters often receive hundreds of resumes for a single job position. Manually reviewing each resume is time-consuming and inefficient. This project builds an **AI-powered Resume Screening System** that automatically analyzes resumes, compares them with a job description, and ranks candidates based on their relevance.

The system uses **Natural Language Processing (NLP)** and **Machine Learning techniques** to evaluate how well each resume matches the required job skills.

---

## Objectives

* Automate the resume screening process.
* Compare candidate resumes with a job description.
* Rank candidates based on similarity scores.
* Identify missing skills for each candidate.
* Reduce manual effort in the recruitment process.

---

## Technologies Used

* **Python** – Main programming language
* **Pandas** – Data handling and preprocessing
* **NumPy** – Numerical operations
* **Scikit-learn** – Machine learning utilities
* **TF-IDF Vectorizer** – Feature extraction from text
* **Cosine Similarity** – Resume-job description matching
* **Regular Expressions (re)** – Text cleaning

---

## Dataset

The project uses a **Resume Dataset (Resume.csv)** containing approximately **2484 resumes**.

Dataset Columns:

* **ID** – Unique identifier for each resume
* **Resume_str** – Resume text content
* **Resume_html** – Resume in HTML format
* **Category** – Job category

For this project, the **Resume_str** column is used because it contains the textual information needed for analysis.

---

## Project Workflow

1. **Dataset Loading**

   * Import the resume dataset using Pandas.

2. **Text Preprocessing**

   * Convert text to lowercase
   * Remove numbers and punctuation
   * Remove extra spaces

3. **Feature Extraction**

   * Convert resume text into numerical vectors using **TF-IDF Vectorizer**.

4. **Similarity Calculation**

   * Compare each resume with the job description using **Cosine Similarity**.

5. **Candidate Ranking**

   * Sort resumes based on similarity scores.

6. **Skill Gap Detection**

   * Identify missing skills from the resume compared to required job skills.

---

## Example Job Description

```
Looking for a Data Scientist with skills in Python,
Machine Learning, SQL, Data Analysis, and Deep Learning.
```

---

## Example Output

```
Top Candidate Ranking
---------------------
Candidate 1
Score: 0.89
Missing Skills: Deep Learning

Candidate 2
Score: 0.85
Missing Skills: SQL

Candidate 3
Score: 0.82
Missing Skills: Data Analysis
```

---

## Installation

Install required Python libraries:

```
pip install pandas numpy scikit-learn
```

---

## How to Run the Project

1. Upload the dataset (`Resume.csv`).
2. Open the project in **Google Colab or Jupyter Notebook**.
3. Run the notebook cells sequentially.
4. The system will analyze resumes and display ranked candidates.

---

## Key Concepts Used

* Natural Language Processing (NLP)
* TF-IDF Feature Extraction
* Cosine Similarity
* Text Preprocessing
* Resume Ranking Algorithms

---

## Applications

* HR recruitment automation
* Resume filtering systems
* Talent acquisition platforms
* AI-based hiring tools

---

## Future Improvements

* Resume parsing from PDF files
* Skill extraction using **spaCy NLP**
* Deep learning models for better accuracy
* Web interface using **Streamlit or Flask**
* Automatic resume recommendations

---


## License

This project is developed for **educational and research purposes**.
