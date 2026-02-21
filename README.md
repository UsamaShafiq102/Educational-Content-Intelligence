# Educational Content Intelligence
### Analyzing Linguistic Complexity and Thematic Diversity in AI-Generated Preschool Stories

**Author:** Muhammad Usama Shafiq
**GitHub:** [UsamaShafiq102](https://github.com/UsamaShafiq102)

---

## Project Overview

This project applies NLP and Unsupervised Machine Learning to analyze AI-generated educational
stories for preschool-aged children. It answers two research questions:

1. Is there a measurable difference in **linguistic complexity** between stories for toddlers vs. preschoolers?
2. Do AI-generated stories naturally cluster into coherent **thematic groups**?

Motivated by the author's professional work on **Preschool Kids Academy** — a published mobile
app featuring an AI Story Bot (live on App Store and Google Play).

---

## Techniques Used

- Flesch-Kincaid Readability Analysis (NLTK)
- TF-IDF Vectorization (scikit-learn)
- Sentence-Transformer Embeddings (all-MiniLM-L6-v2)
- K-Means Clustering + PCA Visualization (scikit-learn)

---

## Quickstart

```bash
# 1. Clone the repository
git clone https://github.com/UsamaShafiq102/educational-content-intelligence.git
cd educational-content-intelligence

# 2. Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate

# 3. Install dependencies
pip3 install -r requirements.txt

# 4. Download NLTK data
python3 -c "import nltk; nltk.download('punkt'); nltk.download('stopwords'); nltk.download('punkt_tab')"

# 5. Generate dataset
python3 generate_data.py

# 6. Open the notebook
jupyter notebook analysis.ipynb
```

Run all cells in order: Kernel → Restart & Run All

---
## Repository Structure

```
educational-content-intelligence/
├── README.md
├── requirements.txt
├── generate_data.py
├── sample_stories.csv
├── analysis.ipynb
└── outputs/
    ├── boxplot_readability.png
    └── cluster_scatter.png
```

---
## App Links

- [Preschool Kids Academy — App Store](https://apps.apple.com/pk/app/abc-mouse-tracing-phonics/id1372481283)
- [Preschool Kids Academy — Google Play](https://play.google.com/store/apps/details?id=com.mobizion.preschoolacademy)
