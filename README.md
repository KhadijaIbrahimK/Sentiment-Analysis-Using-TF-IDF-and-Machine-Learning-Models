🧠 Sentiment Analysis Using TF-IDF and Machine Learning Models
This project performs sentiment analysis on text data using preprocessing, feature extraction (TF-IDF), and classification with Logistic Regression and Multinomial Naive Bayes. The objective is to classify text into different sentiment categories (e.g., positive, neutral, negative) and compare the performance of ML models.

📚 Libraries Used
python
Copy
Edit
nltk, pandas, matplotlib, seaborn, re
wordcloud, sklearn (LogisticRegression, MultinomialNB, metrics, preprocessing, feature_extraction)
📂 Dataset
train.csv and test.csv

Columns: text, selected_text, sentiment

Sentiment classes include: positive, neutral, negative

🧹 Preprocessing Steps
Text Cleaning:

Removed mentions (@), hashtags, URLs, and special characters.

Removed unnecessary whitespace and punctuation.

Converted all text to lowercase.

Stemming & Stopword Removal:

Used PorterStemmer from nltk.

Removed English stopwords using nltk.corpus.stopwords.

Tokenization:

Applied ToktokTokenizer for tokenizing text.

TF-IDF Feature Extraction:

Transformed text into numerical vectors with TfidfVectorizer.

Limited to the top 100,000 features.

📊 Data Visualization
Pie chart showing sentiment distribution in training data.

WordCloud and other exploratory visuals can be added.

Confusion matrix heatmaps for both models.

Bar chart comparing model accuracies.

🤖 Models Implemented
1. Logistic Regression
Used L2 penalty with C=1 and max_iter=500.

Trained using TF-IDF features.

Accuracy: ~71%

2. Multinomial Naive Bayes
Trained using the same TF-IDF vectors.

Accuracy: ~63%

📈 Model Evaluation
Used accuracy_score, confusion_matrix, and classification_report from sklearn.metrics.

Plotted confusion matrices for qualitative performance comparison.

Compared overall accuracies using bar plots.

📷 Screenshots (Optional)
You can insert screenshots of plots and confusion matrices here for visual summary.

🚀 Future Improvements
Include deep learning models (LSTM, BERT).

Hyperparameter tuning using GridSearchCV.

Perform cross-validation for better generalization.

Add more feature engineering (e.g., POS tagging, sentiment lexicons).

