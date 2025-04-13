Text Summarization using BiLSTM, Encoder-Decoder Architecture, and BERT Transformer

✨ Project Overview

Customer reviews, especially on e-commerce platforms, can be lengthy and time-consuming to analyze manually. This project focuses on abstractive text summarization of customer reviews, aiming to generate concise summaries of long review texts automatically.

We leverage two approaches:
	•	Custom BiLSTM Encoder-Decoder Architecture: Built using TensorFlow/Keras for generating summaries.
	•	Pre-trained BERT Transformer (BART): Utilized through Hugging Face’s Transformers library for comparison and enhanced performance.

The project uses the Amazon Fine Food Reviews dataset sourced from Kaggle.

⸻

📚 Problem Statement
	•	Understand the concept of text summarization.
	•	Perform thorough data cleaning and preprocessing.
	•	Implement abstractive summarization using deep learning architectures.
	•	Compare custom models against state-of-the-art transformers.

⸻

🛠️ Technologies Used
	•	Python
	•	TensorFlow / Keras
	•	Hugging Face Transformers
	•	Pandas, NumPy, Matplotlib, Seaborn (for data manipulation and visualization)

⸻

🔗 Dataset

We have used the Amazon Fine Food Reviews dataset available on Kaggle.
This dataset contains 500,000+ food reviews including text, ratings, and summary fields.

⸻

🏗️ Project Pipeline
	1.	Data Collection:
Downloaded using Kaggle API.
	2.	Data Cleaning:
	•	Removed duplicates and NaN values.
	•	Converted all text to lowercase.
	•	Removed HTML tags, special characters, numbers, and text within parentheses.
	•	Added special tokens (sostok, eostok) to summaries.
	3.	Text Preprocessing:
	•	Tokenization.
	•	Sequence padding.
	•	Train-validation split.
	4.	Model Building:
	•	BiLSTM Encoder: Processes input review text.
	•	Decoder with LSTM: Predicts the summary sequence.
	•	Embedding Layer: Learned word representations.
	•	Early Stopping: To avoid overfitting.
	5.	Training:
	•	Trained the BiLSTM model for 20 epochs with validation monitoring.
	6.	Inference:
	•	Built separate encoder and decoder models for generating summaries.
	7.	Transformer Summarization:
	•	Used BART (facebook/bart-large-cnn) from Hugging Face for benchmark summarization.

⸻

📈 Sample Results
	•	Input: “I recently purchased this organic green tea, and I must say, I am thoroughly impressed…”
	•	Generated Summary (BiLSTM Model): great tea
	•	Generated Summary (BART Model): “I drink this tea every morning, and it gives me a calming start to my day…”

⸻

👨‍💻 Authors
	•	Vaishnav Naik
	•	Yashaurya Soni
	•	Piyush Borakhade

⸻

📄 License

This project is for academic purposes only.
