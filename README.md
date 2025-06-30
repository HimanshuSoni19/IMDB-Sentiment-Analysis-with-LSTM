# 🎬 IMDB Sentiment Analysis & Web App Deployment

A machine learning-powered sentiment analysis tool built using IMDB movie reviews. This project uses both traditional ML and deep learning models (Logistic Regression and LSTM) and deploys the final model via a Gradio web interface for real-time sentiment prediction.

---

## 📌 Project Overview

- **Goal**: Predict whether an IMDB movie review is positive or negative.
- **Dataset**: 50,000 labeled reviews from the IMDB dataset.
- **Interface**: Real-time sentiment prediction using Gradio.

---

## 🧠 Models & Techniques

### 1. Data Preprocessing
- Lowercasing, punctuation & stopword removal
- Tokenization and vectorization using:
  - **TF-IDF** for traditional models
  - **Word2Vec** for deep learning

### 2. Models Used
| Model               | Vectorization | Notes                              |
|--------------------|---------------|-------------------------------------|
| Logistic Regression | TF-IDF        | Lightweight & interpretable         |
| Naive Bayes         | TF-IDF        | Baseline performance                |
| LSTM Neural Network | Word2Vec      | Best performance, final model used  |

---

## 💻 Web App Deployment (Gradio)

- **Library**: [Gradio](https://www.gradio.app/)
- **UI**: Textbox input + sentiment output
- **Usage**:
  - Users input a review
  - Model predicts sentiment in real-time
  - Can be launched locally or shared via link

```python
interface.launch(share=True)
