# Replication Package: Mining User Feedback for Software Maintenance and Evolution

This repository contains the replication package, data extraction schemas, analysis scripts, and supplementary materials for the Bachelor's Thesis:

> **"Come migliorare la propria app"**  
> **Candidate:** Giovanni Di Rosa (Matr. 0512117288)  
> **Supervisor:** Prof. Fabio Palomba  
> **Affiliation:** Software Engineering Lab (SeSa Lab), Department of Computer Science, University of Salerno, Italy  
> **Academic Year:** 2025–2026  

---

## 📁 Repository Structure

```text
├── data/
│   ├── raw_search_results/       # Exported queries from IEEE Xplore, ACM DL, SpringerLink, ScienceDirect
│   ├── screening/                # Title/Abstract and Full-Text screening logs (CSV/XLSX)
│   └── extracted_data/           # Structured data extraction tables for the 14 primary studies
├── datasets_metadata/            # Summaries and references for benchmark datasets (Pan, Maalej, CRISTAL, CLAP, Steam, etc.)
├── scripts/                      # Python/R scripts for statistical validation and plotting
│   ├── wilcoxon_cliff_delta.py   # Statistical significance and effect size computation
│   └── plot_comparisons.py       # Performance metric visualizer
├── docs/                         # Study protocol and full inclusion/exclusion checklist
└── README.md                     # Replication instructions and documentation
```

---

## 🔍 Systematic Search Protocol & Query Strings

The systematic literature identification was conducted using the following boolean query:

```text
("app reviews" OR "user feedback" OR "tweets" OR "game reviews" OR "fake reviews") 
AND 
("software maintenance" OR "natural language processing" OR "associative classification" OR "feature selection" OR "traceability" OR "release planning" OR "ethics" OR "sentiment analysis")
```

### Search Results by Database
| Digital Library / Source | Initial Records | Title/Abstract Screened | Full-Text Included |
| :--- | :---: | :---: | :---: |
| **IEEE Xplore** | 412 | 28 | 6 |
| **ACM Digital Library** | 385 | 24 | 4 |
| **SpringerLink / ScienceDirect** | 260 | 15 | 2 |
| **Gray Lit. & Snowballing (Scopus/Scholar)** | 140 | 8 | 2 |
| **Total** | **1,197** | **75** | **14** |

---

## 📊 Benchmark Datasets Included in the Comparative Study

1. **Pan Dataset** (Panichella et al., 2015): 1,390 labeled review sentences across 7 mobile apps.
2. **Maalej Dataset** (Maalej & Nabil, 2015 / Maalej et al., 2016): 3,691 / 4,400 multi-attribute app reviews.
3. **Twitter Technical & Emotion Corpora** (Williams & Mahmoud, 2017): 51,792 technical tweets and 360,873 emotion tweets.
4. **CRISTAL Open-Source Benchmark** (Palomba et al., 2015): 100 Android open-source apps with commit/issue traceability links.
5. **CLAP Release Planning Dataset** (Villarroel et al., 2016): 1,000 classification reviews, 200 clustered reviews, 463 prioritized release reviews across 200+ apps.
6. **Apple App Store Fake Reviews Benchmark** (Martens & Maalej, 2019): 60,000 fake reviews contrasted against 62.6M official reviews.
7. **Steam VGSE Ethics & Longitudinal Corpus** (Voria et al., 2025; Martens & Johann, 2017): 326,440 Steam reviews for ethical taxonomies and 7.37M longitudinal App Store reviews.

---

## ⚙️ How to Replicate Analysis and Statistical Tests

### Prerequisites
* Python 3.9+
* Required packages: `numpy`, `scipy`, `pandas`, `matplotlib`, `seaborn`

```bash
pip install -r requirements.txt
```

### Running Statistical Tests (Wilcoxon Signed-Rank & Cliff's Delta)
To reproduce the statistical validation on Feature Selection (Information Gain vs. Chi-Square):

```bash
python scripts/wilcoxon_cliff_delta.py
```

---

## 📄 License & Attribution
The material in this repository is distributed under the [MIT License](LICENSE). Please cite the thesis and original primary sources when reusing these artifacts.
