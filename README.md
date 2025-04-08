# Cloud-Based NLP Model for Automated Document Summarization

This project is focused on building a scalable, cloud-native NLP system that performs automated document summarization using a fine-tuned transformer model. The solution includes:

- 📄 Text and PDF file upload support
- 🤖 Transformer-based summarization using BART (fine-tuned on CNN/DailyMail)
- 🧪 ROUGE-based evaluation
- 🌐 Flask API for model serving
- 🐳 Docker containerization
- 🔬 Ready for cloud deployment and load testing

---

## ✅ Features

- **Summarization Model**: Fine-tuned `facebook/bart-large-cnn` on CNN/DailyMail dataset
- **File Support**: `.pdf` and `.txt` files via `pdfplumber`
- **API Framework**: Flask with endpoint `/summarize`
- **Deployment**: Docker-ready setup
- **Evaluation**: ROUGE scores computed post-training
- **Temporary Storage**: Files are saved and removed securely
- **Load Testing Preview**: Locust script outline included for traffic simulation

---

## 🧠 Model Training

The model was fine-tuned using Hugging Face's `Trainer` API:

- Dataset: `cnn_dailymail`, version 3.0.0
- Tokenizer: `facebook/bart-large-cnn`
- Max input length: 1024 tokens
- Max output length: 130 tokens

Trained using:
```bash
transformers==4.x
datasets==2.x
torch>=1.10
```

Output saved to:
```bash
./bart-cnn-finetuned/
```

---

## 🔧 Flask API Usage

### Run the app:

```bash
python app.py
```

### Test with CURL:

```bash
curl -X POST -F "file=@sample.pdf" http://localhost:5000/summarize
```

### Sample Output:
```json
{
  "summary": "This model summarizes documents with high accuracy...",
  "original_length": 975,
  "summary_length": 120
}
```

---

## 🐳 Docker Support

### Build Image:

```bash
docker build -t summarizer-api .
```

### Run Container:

```bash
docker run -p 5000:5000 summarizer-api
```

---

## 📈 ROUGE Evaluation

ROUGE-1, ROUGE-2, and ROUGE-L metrics were calculated after training to evaluate summarization quality. Results are available in the `ROGUE_Evaluation_Metrics.ipynb`.

---

## 🛠 Tech Stack

- **Model**: Hugging Face Transformers (`facebook/bart-large-cnn`)
- **Training**: PyTorch + Transformers `Trainer`
- **API**: Flask
- **PDF Extraction**: `pdfplumber`
- **Containerization**: Docker
- **Evaluation**: ROUGE (`datasets`, `evaluate`)
- **Testing**: Locust (optional)

---

## 📁 Project Structure

```
cloud-nlp-summarizer/
│
├── bart-cnn-finetuned/          # Fine-tuned model artifacts
├── app.py                       # Flask API
├── requirements.txt             # Python dependencies
├── docker.txt                   # Dockerfile
├── Base_BART+Finetuning.ipynb   # Training notebook
├── ROGUE_Evaluation_Metrics.ipynb # Evaluation notebook
├── Flask_Using_Finetuned_Model.ipynb # API backend demo
└── Week_4_Cloud_API_and_Docker.ipynb # Docker + deployment guide
```

---

## 🔜 Next Steps

- [ ] Containerize frontend with React + Vite
- [ ] Deploy on GCP or AWS (Cloud Run / ECS / EKS)
- [ ] Add Prometheus + Grafana for monitoring
- [ ] Secure the API with JWT or OAuth

---

## 👨‍💻 Authors

- Ayush Sinha LNU (as1618@umd.edu)
- Siddhardh Chochipatla (schochip@umd.edu)
- Sri Akash Kadali (kadali18@umd.edu)

---
