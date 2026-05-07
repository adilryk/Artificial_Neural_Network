# 🧠 Deep Learning Sentiment Analysis on Women's Clothing Reviews

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python">
  <img src="https://img.shields.io/badge/TensorFlow-DeepLearning-orange?style=for-the-badge&logo=tensorflow">
  <img src="https://img.shields.io/badge/Keras-NeuralNetworks-red?style=for-the-badge&logo=keras">
  <img src="https://img.shields.io/badge/NLP-SentimentAnalysis-green?style=for-the-badge">
</p>

<p align="center">
  A Deep Learning NLP project comparing <strong>CNN</strong> and <strong>LSTM</strong> architectures for sentiment classification on the Women's E-Commerce Clothing Reviews dataset.
</p>

---

# 📌 Project Overview

This project applies advanced **Deep Learning techniques** to classify women's clothing reviews as:

* ✅ Positive Reviews
* ❌ Negative Reviews

The project compares the performance of:

* 🧠 Convolutional Neural Networks (CNN)
* 🔁 Long Short-Term Memory Networks (LSTM)

using Natural Language Processing (NLP) and TensorFlow/Keras.

---

# 📂 Dataset

Dataset Used:

**Women's E-Commerce Clothing Reviews**

* Total Reviews: **22,641**
* Positive Reviews: **17,448**
* Negative Reviews: **5,193**

Dataset Source:

* Kaggle Dataset by `nicapotato`

---

# 🚀 Technologies Used

| Technology         | Purpose                   |
| ------------------ | ------------------------- |
| Python             | Programming Language      |
| TensorFlow / Keras | Deep Learning             |
| Scikit-learn       | Evaluation Metrics        |
| Pandas             | Data Processing           |
| NumPy              | Numerical Computing       |
| Matplotlib         | Visualization             |
| Seaborn            | Statistical Visualization |

---

# 🧹 Data Preprocessing

The following preprocessing steps were applied:

* Removing missing values
* Text tokenization
* Sequence padding
* Binary sentiment labeling
* Train-test split

### Sentiment Mapping

| Rating | Sentiment |
| ------ | --------- |
| 1-3    | Negative  |
| 4-5    | Positive  |

---

# 🔤 NLP Configuration

| Parameter           | Value  |
| ------------------- | ------ |
| Vocabulary Size     | 10,000 |
| Embedding Dimension | 128    |
| Max Sequence Length | 100    |
| Batch Size          | 128    |
| Epochs              | 15     |

---

# 🧠 CNN Model Architecture

```python id="ffy6kq"
Embedding → Conv1D → MaxPooling → Conv1D → MaxPooling → Flatten → Dense → Dropout → Output
```

### CNN Performance

| Metric        | Score  |
| ------------- | ------ |
| Test Accuracy | 86.07% |
| Test Loss     | 1.3898 |

### CNN Classification Report

| Class    | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| Negative | 0.75      | 0.59   | 0.66     |
| Positive | 0.88      | 0.94   | 0.91     |

---

# 🔁 LSTM Model Architecture

```python id="ddu20q"
Embedding → LSTM → Dropout → LSTM → Dense → Output
```

### LSTM Performance

| Metric        | Score  |
| ------------- | ------ |
| Test Accuracy | 87.88% |
| Test Loss     | 0.2799 |

### LSTM Classification Report

| Class    | Precision | Recall | F1-Score |
| -------- | --------- | ------ | -------- |
| Negative | 0.75      | 0.70   | 0.73     |
| Positive | 0.91      | 0.93   | 0.92     |

---

# 📊 Model Comparison

| Model | Accuracy | Best Feature                 |
| ----- | -------- | ---------------------------- |
| CNN   | 86.07%   | Faster Training              |
| LSTM  | 87.88%   | Better Context Understanding |

### 🏆 Best Performing Model: LSTM

The LSTM model achieved higher accuracy and better sentiment understanding compared to CNN.

---

# 📈 Visualizations

The project includes:

* 📊 Sentiment distribution plots
* ⭐ Rating distribution graphs
* 📝 Review length analysis
* 📉 Training vs Validation accuracy/loss
* 🔳 Confusion matrices

---

# 🛠️ Installation

Clone the repository:

```bash id="g0x9w5"
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

Install dependencies:

```bash id="k4e34u"
pip install -r requirements.txt
```

---

# ▶️ Run the Project

```bash id="2qq3wu"
python main.py
```

Or run the notebook directly in:

* Jupyter Notebook
* Google Colab
* Kaggle Notebook

---

# 📦 Required Libraries

```txt id="e6vxg7"
tensorflow
keras
pandas
numpy
matplotlib
seaborn
scikit-learn
kagglehub
```

---

# 📸 Results Preview

## CNN Accuracy

* Training Accuracy reached nearly 100%
* Validation Accuracy stabilized around 85-86%

## LSTM Accuracy

* More stable validation performance
* Better generalization on unseen reviews

---

# 🔮 Future Improvements

* Implement Bidirectional LSTM
* Add GRU architecture
* Use pretrained embeddings (GloVe / Word2Vec)
* Apply Transformer-based models (BERT)
* Hyperparameter optimization
* Deploy as a web application

---

# 👨‍💻 Author

Developed with ❤️ using Deep Learning and NLP

---

# ⭐ Support

If you found this project helpful, please give it a ⭐ on GitHub!

---

# 📜 License

This project is licensed under the MIT License.
