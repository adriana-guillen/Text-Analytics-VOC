💬 Voice of the Customer & Employee – Sentiment Analysis at a Fuel Retail Chain.

**Portfolio Project | Business Analytics | Text Analytics | NLP**

This project simulates a real-world sentiment analysis initiative I led in 2012 at **Oxxo Gas**, a major fuel retail chain in Mexico, owned by **FEMSA**, one of Latin America's largest retail and logistics conglomerates.

The analysis focuses on open-ended feedback gathered from three key sources:

- 🕵️‍♀️ **Mystery Shoppers** (external evaluators)
- 👥 **External Customers** (gas station clients)
- 🧑‍💼 **Internal Employees** (company staff visiting the stations)

The objective is to extract service-quality insights from unstructured comments using **classical NLP techniques** — including **TF-IDF**, **Word2Vec**, and a roadmap to **BERT** — to support data-driven service improvement decisions.

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

## 💡 Key Takeaways

- Word2Vec embeddings captured **context and meaning** better than sparse TF-IDF vectors.
- **Logistic Regression** underperformed on complex sentiment boundaries — while Random Forest generalized well.
- This pipeline can scale across other customer-facing business units for performance monitoring.

---

## 🔄 Next Steps

- Integrate a **fine-tuned BERT classifier** to evaluate performance on ambiguous or subtle feedback.
- Test real-world deployment scenarios (e.g., stream processing, email surveys, internal service audits).

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

```
├── Text Analytics Project VOC.ipynb   # Full analysis
├── OxxoGas_VOC.csv                    # Synthetic dataset
└── README.md                          # Project overview
```

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
