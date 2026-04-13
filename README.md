# ✈️ Sentiment Analysis of Airline Tweets  

## 📌 Project Overview  
This project performs **sentiment classification** on airline-related tweets using a **Bi-directional LSTM** with a custom **attention mechanism**.  
The model predicts whether a tweet's sentiment is:  
- **Negative** 😠  
- **Neutral** 😐  
- **Positive** 😊  

It uses the **Twitter Airline Sentiment dataset** and applies text preprocessing, tokenization, sequence padding, and attention-based LSTM architecture for classification.

---

## 🚀 Features  

### 🗂 Data Preprocessing  
- Lowercasing text  
- Removing URLs and mentions (@user)  
- Removing punctuation and numbers  
- Stopword removal  
- Tokenization  

### 📊 Exploratory Data Analysis (EDA)  
- Sentiment distribution plots  
- Sentiment per airline  
- Word cloud visualization  

### 🧠 Deep Learning Architecture  
- Tokenizer-based vocabulary creation  
- Sequence padding for uniform input length  
- **Bi-directional LSTM** for capturing context  
- **Custom Attention Mechanism** to focus on key words  
- Dense output layer with **Softmax activation**  

### 📈 Evaluation  
- Accuracy computation  
- Prediction histograms  

---

## 🛠️ Tech Stack  
- **Python**: NumPy, Pandas, Matplotlib, Seaborn  
- **Text Processing**: Scikit-learn, NLTK, CountVectorizer, Tokenizer  
- **Deep Learning**: TensorFlow / Keras  
- **Visualization**: WordCloud, Matplotlib, Seaborn  

---

## 📂 Dataset  
- **Name**: Twitter Airline Sentiment  
- **Labels**: `negative`, `neutral`, `positive`  
- **Source**: [Kaggle - Twitter Airline Sentiment](https://www.kaggle.com/crowdflower/twitter-airline-sentiment)  

---

## ⚙️ Installation & Setup  

1️⃣ **Clone the repository**  
```bash
git clone https://github.com/yourusername/sentiment-analysis-airline.git
cd sentiment-analysis-airline
```
2️⃣ **Install dependencies**
```bash
pip install -r requirements.txt
```
3️⃣ **Download dataset from Kaggle and place tweets.csv in the project folder.**
4️⃣ **Run the notebook**
```bash
jupyter notebook sentiment_analysis.ipynb
```
---
# 📊 Model Architecture

**Architecture Flow:**
```css
Input Tweets → Tokenization → Padding → Embedding Layer →
Bi-Directional LSTM → Attention Layer → Dense Layer (Softmax)
```
---
# 🧪 Sample Predictions
| Tweet                                                  | Predicted Sentiment | Confidence |
| ------------------------------------------------------ | ------------------- | ---------- |
| The flight was delayed for 3 hours, terrible service!  | Negative            | 0.95       |
| Staff was polite and boarding was smooth.              | Positive            | 0.91       |
| It was an average experience, nothing special.         | Neutral             | 0.76       |
| I will never fly with them again. Absolutely horrible. | Negative            | 0.97       |
| Loved the extra legroom and friendly crew!             | Positive            | 0.93       |
---
# 📈 Results
**Achieves 77.82% accuracy on the validation set**

**Visualizations show clear separation between negative and positive tweets**

---
# 🔮 Future Improvements
**Experiment with BERT-based embeddings for richer context**

**Add hyperparameter tuning with KerasTuner**

**Deploy as a Flask API or Streamlit app**

---

## License
This project is licensed under the [MIT License](./LICENSE) — Copyright (c) 2026 Swati Shekhawat
