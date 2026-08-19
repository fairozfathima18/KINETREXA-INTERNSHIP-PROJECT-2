# Resume Screening & Candidate Recommendation System

## Overview

An NLP and Machine Learning recruitment system that extracts skills, compares candidates with a job description, ranks candidates, and recommends suitable candidates.

This version is designed for **Jupyter Notebook** and does not require Streamlit or TensorFlow.

## Features

* Candidate/resume data processing
* NLP text preprocessing
* Skill extraction
* TF-IDF vectorization
* Cosine similarity
* Candidate ranking
* Recommendation engine

## Technology Stack

Python, Jupyter Notebook, Pandas, NumPy, Scikit-learn, Matplotlib, Regular Expressions.

## Dataset

The CSV contains 20 demo candidates with:

* CandidateID
* Name
* Skills
* Education
* ExperienceYears
* TargetRole
* Email

## How to Run

1. Keep the Jupyter notebook and CSV in the same folder.
2. Open the notebook in Jupyter/JupyterLab.
3. Run cells from top to bottom.
4. Change the `job_description` variable to test different jobs.
5. View extracted skills, similarity scores, matched skills, rankings, and the top recommendation.

## Methodology

1. Load candidate CSV.
2. Clean text.
3. Extract skills using a predefined skill vocabulary.
4. Convert job and candidate text into TF-IDF vectors.
5. Calculate cosine similarity.
6. Find matched skills.
7. Rank candidates.
8. Display recommendations.

## Algorithm

```text
Job Description
      ↓
Text Preprocessing
      ↓
Skill Extraction
      ↓
TF-IDF Vectorization
      ↓
Cosine Similarity
      ↓
Candidate Ranking
      ↓
Recommendation
```

## Required Packages

`pandas`, `numpy`, `scikit-learn`, `matplotlib`.

If normal pip is available:

```python
%pip install pandas numpy scikit-learn matplotlib
```

**TensorFlow and Streamlit are not required for the Jupyter version.**

## Future Enhancements

* PDF/DOCX resume parsing
* spaCy NER
* Sentence-BERT embeddings
* Experience/education weighting
* Database integration
* Recruiter dashboard
* Authentication
* Explainable AI
* Fairness evaluation
* Cloud deployment

## Limitation

This is an educational prototype using structured candidate profiles and a predefined skill vocabulary. Recommendations should support human review, not replace it.
