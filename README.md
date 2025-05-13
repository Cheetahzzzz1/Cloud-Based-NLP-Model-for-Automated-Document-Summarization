# 🧠 Text Summarization NLP App

An AI-powered tool to simplify **text analysis** and **document summarization** using cutting-edge Natural Language Processing (NLP) techniques. With just a few clicks, you can generate summaries, detect sentiment, and visualize text insights, making it easy to process and understand large volumes of content.

---

## 🚀 Features

- 📝 **Text Summarization**  
  Generate concise, relevant summaries using either:
  - Frequency-based NLP methods
  - Pegasus (transformer-based) model via API toggle

- 📊 **Sentiment Analysis**  
  Analyze emotional tone — positive, negative, or neutral — using VADER.

- ☁️ **Word Cloud Generation**  
  Visualize high-frequency terms in your text using intuitive word clouds.

- 📄 **PDF Upload Support**  
  Upload and extract text directly from PDF files for all actions.

- ⚙️ **Light/Dark Mode UI**  
  Beautiful theme toggle with responsive, modern design.

---

## 🧪 Usage Guide

1. **Summarization**  
   Paste text or upload a PDF → choose summarization → select Pegasus or traditional method → get instant output.

2. **Sentiment Analysis**  
   The app uses VADER to compute compound polarity scores and charts the emotional tone.

3. **Word Cloud**  
   Generates a word cloud highlighting the most frequent non-stop words.

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

![Home](https://github.com/user-attachments/assets/4eb869f3-c26b-48b2-82fb-ece5bb8debff/static/1.png)

### 🔹 Text Summarization

![Summarization](https://github.com/user-attachments/assets/9c6424b0-5eb6-4977-bf38-fca1691587f0/static/2.png)

### 🔹 Sentiment Analysis

![Sentiment](https://github.com/user-attachments/assets/ba7bfd15-a683-494f-9aa6-fa3207b280c1/static/3.png)

### 🔹 Word Cloud

![Word Cloud](https://github.com/user-attachments/assets/8ac1b2c7-c4dc-436f-b54e-da37aa19b3d5/static/4.png)

---

## 🔧 Tech Stack

* **Backend:** Flask
* **NLP:** NLTK, VADER, SentencePiece, Transformers
* **Visualization:** Matplotlib, WordCloud, Chart.js
* **Cloud Inference:** Pegasus model via Modal API

---

## 📄 License

MIT License — free for personal and commercial use. Attribution appreciated.

---

> Designed & Developed by **Sri Akash Kadali** ✨
> Empowering faster reading, smarter decisions.
