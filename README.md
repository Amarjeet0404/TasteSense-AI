# TasteSense-AI

# 🍽️ TasteSense AI  
**AI-Powered Sentiment Analysis & Topic Modeling for Yelp Reviews**  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
![SpaCy](https://img.shields.io/badge/NLP-SpaCy-green)  
![HuggingFace](https://img.shields.io/badge/Transformers-BERT-orange)  
![LDA](https://img.shields.io/badge/Topic%20Modeling-LDA-yellow)  

---

## 📌 Overview  
TasteSense AI is an **intelligent review analysis system** designed to help **restaurants and businesses** gain actionable insights from large volumes of Yelp reviews.  
It leverages **NLP, BERT-based sentiment analysis, and topic modeling** to deliver **real-time insights** into customer feedback.  

---

## ✅ Features  
✔ Automatic **Sentiment Detection** (Positive / Negative) using **HuggingFace Transformers**  
✔ **Topic Identification** – Food Quality, Service, Pricing, Ambiance, Wait Time  
✔ **Complaint Keyword Extraction** – Detect frequent negative issues  
✔ **Visual Insights** – Pie charts and bar charts for sentiment & topic distribution  
✔ **Faster Decision-Making** through **intelligent analytics**  

---

## 🔍 Problem Statement  
Restaurants receive thousands of unstructured reviews daily.  
- **Manual analysis** is time-consuming and inefficient.  
- **Key issues** (e.g., poor service, pricing complaints) often go unnoticed.  

---

## 💡 Solution – TasteSense AI  
TasteSense AI provides:  
- ✅ **BERT-powered Sentiment Analysis**  
- ✅ **Topic Modeling with LDA** for hidden trends  
- ✅ **Visualizations for actionable insights**  
- ✅ **Keyword extraction from negative reviews**  

---

## 🛠 Tech Stack  
- **Python 3.8+**  
- **SpaCy** (Text Preprocessing)  
- **Hugging Face Transformers** (distilbert-base-uncased-finetuned-sst-2-english)  
- **Scikit-learn** (TF-IDF Vectorization)  
- **LDA** (Topic Modeling)  
- **Matplotlib / Seaborn** (Visualization)  
- **Pandas / NumPy** (Data Handling)  

---

## 📂 Project Workflow  

### **1. Data Acquisition**  
- Load Yelp review dataset (JSON format)  
- Each review includes **rating (stars)** and **text feedback**  
- Use a **sample of 100 reviews** for demo/testing  

### **2. Text Preprocessing**  
- **SpaCy (en_core_web_sm)** for:  
  ✔ Tokenization  
  ✔ Stopword Removal  
  ✔ Punctuation Removal  
  ✔ Lemmatization  
- Generate **cleaned text** for NLP models  

### **3. Sentiment Classification**  
- **Model:** `distilbert-base-uncased-finetuned-sst-2-english`  
- Outputs:  
  ✔ **Sentiment Label** (Positive / Negative)  
  ✔ **Confidence Score**  
- Store results as **new columns** in the dataset  

### **4. Topic Modeling**  
- **TF-IDF Vectorization** → Convert text to numerical vectors  
- **LDA (Latent Dirichlet Allocation)** → Extract hidden topics  
- Topics identified:  
  ✔ Food Quality  
  ✔ Service  
  ✔ Pricing  
  ✔ Ambiance  
  ✔ Wait Time  

### **5. Insights & Visualization**  
- **Pie Chart:** Overall sentiment distribution  
- **Stacked Bar Chart:** Topic-wise sentiment breakdown  
- **Keyword Extraction:** Detect frequent complaints from negative reviews  



