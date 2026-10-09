<div align="center">

# 😊 Text Polarity (Sentiment) Detection

**A text-CNN built with TensorFlow that decides whether a review is positive or negative.**

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-NLP-informational)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

</div>

---

## ✨ Overview

`polaritydetection.ipynb`:

1. 🧹 **Preprocess** the texts - tokenize with NLTK, remove stop words and punctuation, shuffle the data.
2. 🔢 **Vectorize** with the Keras `Tokenizer` and `pad_sequences`.
3. 🧠 **Model** - an `Embedding` layer followed by `Conv1D` + `MaxPool1D` branches (a *Text-CNN*) and dense layers, trained for 10 epochs; validation accuracy is about **84 %**.
4. 💾 Saves the model (`textcnn.h5`) and the tokenizer, then reloads them to classify new sentences.

## 🚀 Getting Started

```bash
git clone https://github.com/Arashomranpour/PolarityDetection.git
cd PolarityDetection
pip install tensorflow nltk numpy jupyter
python -c "import nltk; nltk.download('stopwords'); nltk.download('punkt')"
jupyter notebook polaritydetection.ipynb
```

Point the data-loading cell at your own labelled positive / negative text files.

## 📁 Project Structure

```
.
└── polaritydetection.ipynb
```

## 🛠️ Tech Stack

`TensorFlow / Keras` · `NLTK` · `NumPy`
