# Resume-Ranker

A smart resume ranking system that uses advanced NLP techniques — including **BERTopic** and **TF-IDF** — to analyze, cluster, and rank resumes based on semantic similarity to a job description.

---

## 🚀 Features

- 🔍 Extracts and analyzes topics from resume content.
- 🧠 Leverages **BERTopic** for contextual topic modeling.
- 📊 Ranks resumes based on similarity to job requirements.
- ✅ Compatible with Google Colab or local Python environments.

---

## 📦 Model Files (Stored on Google Drive)

Due to GitHub file size limits, pretrained models are stored externally.

🔗 [📁 Download Model Files](https://drive.google.com/drive/folders/1DQjgr5Rh40vHfrbBa6bf9eCc-e0Nycrs?usp=sharing)

Files include:
- `sentence_bert_model.zip`
- `tfidf_vectorizer.zip`

---

## 🔧 How to Use

### Option 1: Use in Google Colab

You can run the notebook directly in [Google Colab]([https://colab.research.google.com/](https://colab.research.google.com/drive/13fKvhO0rKVRqCYA0CIjSKodHZGcA3ijw?usp=sharing)):
```
# Install required tools

!pip install gdown

# Download from Google Drive

import gdown, zipfile
gdown.download_folder("https://drive.google.com/drive/folders/1DQjgr5Rh40vHfrbBa6bf9eCc-e0Nycrs", quiet=False)

# Unzip models

with zipfile.ZipFile("sentence_bert_model.zip", 'r') as zip_ref:
    zip_ref.extractall("sentence_bert_model")

with zipfile.ZipFile("tfidf_vectorizer.zip", 'r') as zip_ref:
    zip_ref.extractall("tfidf_vectorizer")
```

### Option 2: Run Locally
Clone the repo:
```
git clone https://github.com/Neel77Mahi/Resume-Ranker.git
cd Resume-Ranker
```
Install dependencies:
```
pip install -r requirements.txt
Manually download and extract the model files from the Drive link into the project directory.
```
---

🛠️ Requirements

bertopic
umap-learn
hdbscan
gdown
scikit-learn
pandas
matplotlib

Install with:
```
pip install -r requirements.txt
```

Credits
Built by @Neel77Mahi

Powered by BERTopic
