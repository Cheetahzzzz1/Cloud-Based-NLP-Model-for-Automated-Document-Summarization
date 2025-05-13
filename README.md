# 🧠 Text Summarization NLP App

An AI-powered tool to simplify **text analysis** and **document summarization** using cutting-edge Natural Language Processing (NLP) techniques. With just a few clicks, you can generate summaries, detect sentiment, and visualize text insights, making it easy to process and understand large volumes of content.

---

## 🚀 Features

- 📝 **Text Summarization**  
  Generate concise, relevant summaries using either:
  - Frequency-based NLP methods
  - Pegasus (transformer-based) model via Modal API

- 📊 **Sentiment Analysis**  
  Analyze emotional tone — positive, negative, or neutral — using VADER.

- ☁️ **Word Cloud Generation**  
  Visualize high-frequency terms in your text using intuitive word clouds.

- 📄 **PDF Upload Support**  
  Upload and extract text directly from PDF files for all actions.

- 🌗 **Light/Dark Mode UI**  
  Modern responsive interface with a glowing aesthetic and theme toggle.

---

## 🧪 Usage Guide

1. **Summarization**  
   Paste text or upload a PDF → choose summarization → select Pegasus or frequency-based → view results.

2. **Sentiment Analysis**  
   Uses VADER to compute compound polarity scores and visualize via Chart.js.

3. **Word Cloud**  
   Instantly generates a word cloud for the most frequent non-stop words.

---

## 📦 Requirements

**Python Version:** `3.10` to `3.11`

### Install dependencies:
```bash
pip install -r requirements.txt
````

### Run the application:

```bash
python app.py
```

---

## 🌐 UI Snapshots

### 🔹 Home Page

![Home](https://raw.githubusercontent.com/Akash-Kadali/Cloud-Based-NLP-Model-for-Automated-Document-Summarization/main/static/2.png)

### 🔹 Text Summarization

![Summarization](https://raw.githubusercontent.com/Akash-Kadali/Cloud-Based-NLP-Model-for-Automated-Document-Summarization/main/static/1.png)

### 🔹 Sentiment Analysis

![Sentiment](https://raw.githubusercontent.com/Akash-Kadali/Cloud-Based-NLP-Model-for-Automated-Document-Summarization/main/static/4.png)

### 🔹 Word Cloud

![Word Cloud](https://raw.githubusercontent.com/Akash-Kadali/Cloud-Based-NLP-Model-for-Automated-Document-Summarization/main/static/3.png)

---

## 🔧 Tech Stack

* **Backend:** Flask
* **NLP:** NLTK, VADER, Transformers, SentencePiece
* **Visualization:** Matplotlib, WordCloud, Chart.js
* **Cloud Inference:** Pegasus model via Modal API

---

## 📄 License

MIT License — free for personal and commercial use. Attribution appreciated.

---

> Designed & Developed by **Sri Akash Kadali** ✨
> Empowering faster reading, smarter decisions.
