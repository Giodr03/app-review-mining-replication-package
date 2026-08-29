# Replication Package: Mining User Feedback for Software Maintenance and Evolution

This repository contains the replication package, literature corpus, and methodological artifacts for the Bachelor's Thesis:

> **"Come migliorare la propria app"**  
> **Candidate:** Giovanni Di Rosa (Matr. 0512117288)  
> **Supervisor:** Prof. Fabio Palomba  
> **Affiliation:** Software Engineering Lab (SeSa Lab), Department of Computer Science, University of Salerno, Italy  
> **Academic Year:** 2025–2026  

---

## 📁 Repository Structure

```text
├── papers/                                                   # Full-text PDFs of the 14 primary and foundational studies
│   ├── 2884781.2884818.pdf                                   # Villarroel et al. (CLAP, ICSE 2016)
│   ├── 335191.335372.pdf                                     # Han et al. (FP-growth, SIGMOD 2000)
│   ├── Analyzing_Classifying_and_Interpreting_Emotions...    # Williams & Mahmoud (SEmotion 2017)
│   ├── Bug_report_feature_request_or_simply_praise...        # Maalej & Nabil (RE 2015)
│   ├── CMAR_accurate_and_efficient_classification...         # Li et al. (CMAR, ICDM 2001)
│   ├── How_Do_Users_Like_This_Feature...                     # Guzman & Maalej (RE 2014)
│   ├── How_can_i_improve_my_app_Classifying_user_reviews...   # Panichella et al. (ICSME 2015)
│   ├── KDD98-012.pdf                                         # Liu et al. (CBA, KDD 1998)
│   ├── Mining_Twitter_Data_for_a_More_Responsive...          # Williams & Mahmoud (ICSE-C 2017)
│   ├── On_the_Emotion_of_Users_in_App_Reviews.pdf            # Martens & Johann (SEmotion 2017)
│   ├── User_reviews_matter_Tracking_crowdsourced_reviews...  # Palomba et al. (CRISTAL, ICSME 2015)
│   ├── _TOSEM__GV__Ethical_Concern_in_Video_Games...         # Voria et al. (TOSEM 2025)
│   ├── s10664-019-09706-9.pdf                                # Martens & Maalej (EMSE 2019)
│   └── s11219-020-09529-8.pdf                                # Al-Hawari et al. (SQJ 2021)
├── LICENSE                                                   # MIT License file
└── README.md                                                 # Replication instructions and documentation
```

---

## 📚 Primary Papers Included (`/papers`)

1. **Panichella et al. (2015)** – *How Can I Improve My App? Classifying User Reviews for Software Maintenance and Evolution* (ICSME 2015)[cite: 1, 10]
2. **Al-Hawari et al. (2021)** – *Classification of Application Reviews into Software Maintenance Tasks Using Data Mining Techniques* (SQJ 2021)[cite: 10]
3. **Williams & Mahmoud (2017)** – *Mining Twitter Data for a More Responsive Software Engineering Process* (ICSE-C 2017)[cite: 10]
4. **Maalej & Nabil (2015)** – *Bug Report, Feature Request, or Simply Praise? On Automatically Classifying App Reviews* (RE 2015)[cite: 10]
5. **Guzman & Maalej (2014)** – *How Do Users Like This Feature? A Fine Grained Sentiment Analysis of App Reviews* (RE 2014)[cite: 10]
6. **Martens & Johann (2017)** – *On the Emotion of Users in App Reviews* (SEmotion 2017)[cite: 10]
7. **Williams & Mahmoud (2017)** – *Analyzing, Classifying, and Interpreting Emotions in Software Users' Tweets* (SEmotion 2017)[cite: 10]
8. **Voria et al. (2025)** – *Ethical Issues in Video Games: A Large-Scale Empirical Analysis of Gamers' Reviews* (TOSEM 2025)[cite: 10]
9. **Palomba et al. (2015)** – *User Reviews Matter! Tracking Crowdsourced Reviews to Support Evolution of Successful Apps* (CRISTAL, ICSME 2015)[cite: 4, 10]
10. **Villarroel et al. (2016)** – *Release Planning of Mobile Apps Based on User Reviews* (CLAP, ICSE 2016)[cite: 3, 10]
11. **Martens & Maalej (2019)** – *Towards Understanding and Detecting Fake Reviews in App Stores* (EMSE 2019)[cite: 5, 10]
12. **Liu et al. (1998)** – *Integrating Classification and Association Rule Mining* (CBA, KDD 1998)[cite: 10]
13. **Han et al. (2000)** – *Mining Frequent Patterns Without Candidate Generation* (FP-growth, SIGMOD 2000)[cite: 10]
14. **Li et al. (2001)** – *CMAR: Accurate and Efficient Classification Based on Multiple Class-Association Rules* (ICDM 2001)[cite: 10]

---

## 🔍 Search Strategy & Selection Protocol

The systematic literature identification was executed across digital libraries using the combined boolean query[cite: 10]:

("app reviews" OR "user feedback" OR "tweets" OR "game reviews" OR "fake reviews")
AND
("software maintenance" OR "natural language processing" OR "associative classification" OR "feature selection" OR "traceability" OR "release planning" OR "ethics" OR "sentiment analysis")


### Identification & Screening Flow
* **Initial Records Retrieved:** 1,197 (IEEE Xplore: 412, ACM DL: 385, SpringerLink/ScienceDirect: 260, Gray Literature & Snowballing: 140)[cite: 10]
* **Duplicates Removed:** 307 (890 unique records retained)[cite: 10]
* **Title/Abstract Screening:** 75 candidate studies selected[cite: 10]
* **Full-Text Eligibility Assessment:** 32 studies examined[cite: 10]
* **Final Primary Selection:** 14 primary studies and methodological foundations[cite: 10]

---

## 🎯 Research Questions Addressed

* **RQ1 (Multimodal Classification & NLP):** Impact of integrating NLP syntactic patterns, text analysis (TA), and sentiment analysis (SA) compared to single-technique baselines[cite: 10].
* **RQ2 (Associative Classification & Feature Selection):** Performance, rule interpretability (CARs), and compression efficiency of associative algorithms (ACRM, CBA, CBA2, CMAR, CPAR) and feature selection methods (Information Gain, Chi-Square)[cite: 10].
* **RQ3 (Traceability, Release Planning & Data Integrity):** Linking user feedback to source code changes (CRISTAL)[cite: 4, 10], clustering and release prioritization (CLAP)[cite: 3, 10], and detecting incentivized/fake reviews[cite: 5, 10].
* **RQ4 (Ethics, Emotions & Domain Engineering):** Categorization of ethical concerns across software lifecycles and temporal tracking of emotional dynamics in user feedback (VGSE & App Stores)[cite: 10].

---

## 📊 Benchmark Datasets Referenced

* **Pan Dataset:** 1,390 review sentences labeled into 4 maintenance intentions[cite: 10].
* **Maalej Dataset:** 3,691 / 4,400 app reviews classified into 4 stakeholder-oriented categories[cite: 10].
* **Twitter Corpora:** 51,792 technical tweets and 360,873 emotion-annotated tweets[cite: 10].
* **CRISTAL Open-Source Benchmark:** 100 open-source Android applications mapped to commit and issue logs[cite: 4, 10].
* **CLAP Dataset:** 1,000 classification reviews, 200 clustered reviews, and 463 prioritized reviews across 200+ mobile apps[cite: 3, 10].
* **Apple App Store Fake Reviews Benchmark:** 60,000 fake reviews contrasted against 62.6M official store reviews[cite: 5, 10].
* **Steam VGSE & Longitudinal Corpus:** 326,440 Steam game reviews mapped to 19 ethical dimensions and 7.37M longitudinal App Store reviews[cite: 10].

---

## 📄 License & Attribution
The documentation and artifacts in this repository are distributed under the [MIT License](LICENSE). Please cite the thesis and original primary sources when reusing these artifacts.
