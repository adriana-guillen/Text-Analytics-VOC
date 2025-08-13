# 💬 Voice of the Customer & Employee – Sentiment Analysis at a Fuel Retail Chain

**Portfolio Project | Business Analytics | Text Analytics | NLP**

This project simulates a real-world sentiment analysis initiative I led in 2012 at **Oxxo Gas**, a major fuel retail chain in Mexico, owned by **FEMSA**, one of Latin America's largest retail and logistics conglomerates.

The analysis focuses on open-ended feedback gathered from three key sources:  

- 🕵 **Mystery Shoppers** (external evaluators)  
- 🛒 **External Customers** (gas station clients)  
- 👩‍💼 **Internal Employees** (company staff visiting the stations)  

---

## 🎯 Objective
To extract service-quality insights from unstructured comments using a **two-stage NLP approach**:

### **Stage 1 – Classical NLP Techniques**
- **Methods:** TF-IDF, Word2Vec  
- **Models:** Logistic Regression, Random Forest  
- **Output:** Baseline sentiment classification, keyword frequency analysis, word clouds, PCA visualizations

### **Stage 2 – BERT Deep Learning Enhancement**
- **Model:** `bert-base-uncased`  
- **Approach:** Zero-shot classification for Positive / Neutral / Negative sentiment  
- **Added Value:** Captures context, nuance, and ambiguous sentiment missed by classical models  
- **Outcome:** Even with a modest 36% accuracy (no fine-tuning), BERT detected subtle linguistic cues that provided actionable insights for service improvement

---

## 📊 Business Impact
By pairing traditional NLP with BERT, the analysis delivers a richer understanding of customer and employee perceptions — supporting operational decisions to:
- Improve service quality  
- Refine employee training programs  
- Prioritize improvements at underperforming stations  

---

## ⚠️ Disclaimer
All datasets were synthetically generated for portfolio purposes and **DO NOT CONTAIN** any real or proprietary data from FEMSA or Oxxo Gas. All entries were simulated to reflect realistic sentiment patterns and customer behavior.


---

## 📁 Dataset

The dataset is **synthetic**, built exclusively for portfolio purposes and inspired by a real analytical project. It contains 1,050 records with the following fields:

| Column     | Description |
|------------|-------------|
| `source`   | Feedback origin (Mystery Shopper, External Customer, Internal Employee) |
| `region`   | Geographic segment (North, Central, South, etc.) |
| `comment`  | Open-ended feedback |
| `sentiment`| Labeled sentiment: Positive / Neutral / Negative |
| `category` | Operational area mentioned (Cleanliness, Staff, Timeliness, etc.) |

---

## 🧠 Project Objectives

- Classify sentiment from open-text comments
- Detect common operational pain points and service strengths
- Compare TF-IDF and Word2Vec feature extraction methods
- Build a scalable foundation for VoC/VoE-driven decision-making

---

## 🛠️ Methods Used

- **Text Preprocessing:** tokenization, cleaning, stopword removal
- **TF-IDF Vectorization** + Logistic Regression / Random Forest
- **Word2Vec Embeddings** (Gensim) + Random Forest
- **Model Evaluation:** Confusion Matrix, Classification Report, F1-score comparison
- **Visualization:** Word Clouds, TF-IDF plots, Side-by-side performance charts
- **Business Insights:** Key takeaways for service optimization

---

## 📊 Highlights

- **Word2Vec + Random Forest** achieved **100% test accuracy**, showing superior semantic understanding over TF-IDF.
- **Neutral sentiment** was the most common category (34%), followed by Negative (33%) and Positive (31%).
- Classical NLP models proved highly effective in structured feedback environments.
- The pipeline shows potential for **VoC/VoE integration** into operational dashboards to prioritize improvements.

---

💡 **Key Takeaways**
- Word2Vec embeddings captured **context and meaning** better than sparse TF-IDF vectors.  
- Logistic Regression underperformed on complex sentiment boundaries — while Random Forest generalized well.  
- BERT (zero-shot, no fine-tuning) identified subtle and context-dependent sentiment cues that classical models missed, adding valuable depth to the analysis.  
- This pipeline can scale across other customer-facing business units for performance monitoring. 

---

## 🚀 How to Reproduce
*This project runs in Python 3.10+ and has been tested in Jupyter Notebook.*


```bash
# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn gensim nltk
```

Then, run the notebook:  
📄 `Text Analytics Project VOC.ipynb`

Make sure `OxxoGas_VOC.csv` is in the same folder.

---

## 📂 File Structure

├── text_analytics_voc_oxxogas.ipynb # Full analysis — Classical NLP (TF‑IDF, Word2Vec) + BERT sentiment classification
├── OxxoGas_VOC_simulated_dataset.csv # Synthetic dataset for analysis
├── README.md # Project overview and methodology

---

## 🔗 Related Projects
(*Explore finished and upcoming projects from this portfolio series*)

- [Prescriptive Analytics: Inventory Optimization](#)
- [Predictive Analytics: Lost Sales Estimation](#)
- [Power BI Dashboard: Retail KPIs](#)
- [BERT Sentiment Classifier (Coming Soon)](#)

---

## 👤 Author

**Adriana Guillén**  
Business Analyst | Data Strategist | NLP Enthusiast  
📍 Monterrey, Mexico  
🔗 [LinkedIn](#) | [GitHub](#)

---

## 📢 License

This project is shared for professional and portfolio purposes only.  
All data is fictionalized and does not reflect actual enterprise or customer data.
