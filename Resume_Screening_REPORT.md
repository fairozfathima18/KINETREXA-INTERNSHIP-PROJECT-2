# PROJECT REPORT
# Resume Screening & Candidate Recommendation System

## 1. Abstract
The Resume Screening & Candidate Recommendation System is an NLP and Machine Learning project that automates the initial stage of recruitment. It compares candidate skills with job requirements, calculates similarity, ranks candidates, and recommends suitable candidates.

## 2. Problem Statement
Manual resume screening is time-consuming when many candidates apply for a position. The system provides an automated first-level screening approach using NLP and text similarity.

## 3. Objectives
1. Process candidate profile information.
2. Extract technical skills.
3. Analyze job descriptions.
4. Calculate candidate-job similarity.
5. Rank candidates.
6. Recommend suitable candidates.

## 4. Proposed System
The system cleans text, extracts skills, creates TF-IDF vectors, calculates cosine similarity, and ranks candidates according to relevance.

## 5. System Architecture
```text
+----------------------+
| Recruiter / HR       |
+----------+-----------+
           |
           v
+----------------------+
| Job Description      |
+----------+-----------+
           |
           v
+----------------------+
| NLP Preprocessing    |
+----------+-----------+
           |
           v
+----------------------+
| Skill Extraction     |
+----------+-----------+
           |
           v
+----------------------+
| TF-IDF Vectorization |
+----------+-----------+
           |
           v
+----------------------+
| Cosine Similarity    |
+----------+-----------+
           |
           v
+----------------------+
| Candidate Ranking    |
+----------+-----------+
           |
           v
+----------------------+
| Recommendation       |
+----------------------+
```

## 6. Modules
### Candidate Data Processing
Candidate information is stored in the CSV dataset.

### NLP Preprocessing
Text is converted to lowercase and normalized.

### Skill Extraction
A predefined vocabulary identifies technical skills.

### TF-IDF
TF-IDF converts job and candidate text into numerical feature vectors.

### Cosine Similarity
The similarity formula is:

`Cosine Similarity(A,B) = (A · B) / (||A|| × ||B||)`

A higher value indicates a closer textual match.

### Candidate Ranking
Candidates are sorted using similarity score and matched-skill count.

### Recommendation Engine
The highest-ranked candidates are presented as recommendations.

## 7. Dataset
The demo dataset contains 20 candidates covering ML, NLP, Data Analytics, AI, Software Development, Cybersecurity, Cloud, DevOps, and related roles.

Fields include CandidateID, Name, Skills, Education, ExperienceYears, TargetRole, and Email.

## 8. Software Requirements
- Python 3.x
- Jupyter Notebook/JupyterLab
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

## 9. Hardware Requirements
- 4 GB RAM or higher
- Dual-core processor or better
- 1 GB free storage
- Web browser

## 10. Working Procedure
1. Load candidate data.
2. Enter a job description.
3. Preprocess text.
4. Extract required skills.
5. Generate TF-IDF vectors.
6. Calculate cosine similarity.
7. Identify matched skills.
8. Rank candidates.
9. Display recommendations.

## 11. Advantages
- Reduces initial screening effort.
- Produces ranked candidates.
- Provides similarity scores.
- Uses interpretable NLP techniques.
- Easy to demonstrate in Jupyter.
- Can be extended with advanced models.

## 12. Limitations
- Demo uses structured profiles rather than actual PDF/DOCX resumes.
- Skill extraction uses a predefined vocabulary.
- TF-IDF has limited semantic understanding.
- Similarity should not be the sole hiring decision.
- No production database or authentication.

## 13. Future Scope
- PDF/DOCX parsing
- spaCy-based NLP
- Sentence-BERT semantic matching
- Experience and education weighting
- Certification/project matching
- Database integration
- Recruiter dashboard
- Authentication
- Explainable recommendations
- Bias/fairness monitoring
- Cloud deployment

## 14. Ethical Considerations
Automated recruitment may introduce bias. The system should be used as decision support with human review, and candidate information must be handled securely.

## 15. Expected Result
The system produces a ranked candidate table containing candidate name, role, matched skills, and similarity score. The strongest match is shown as the top recommendation.

## 16. Conclusion
The project demonstrates how NLP and Machine Learning can support recruitment screening. TF-IDF and cosine similarity provide a simple baseline that can later be upgraded with resume parsing, transformer embeddings, databases, dashboards, and fairness-aware evaluation.

## 17. References
1. Scikit-learn documentation.
2. Pandas documentation.
3. Python documentation.
4. Jurafsky and Martin, Speech and Language Processing.
