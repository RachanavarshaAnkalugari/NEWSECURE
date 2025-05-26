# NEWSECURE
This project detects fake news using ML by preprocessing text, extracting TF-IDF features, and classifying with a Random Forest model. It displays probability scores for each article, and if classified as fake, it generates the article’s IP address to help trace the source of misinformation.
📰 NewSecure: Fake News Detection System
Overview
NewSecure is a machine learning-based application designed to detect fake news from real news articles. It uses a trained Random Forest classifier for accurate classification. The system not only provides a prediction label but also shows the probability scores indicating confidence. If an article is predicted as fake, the system additionally fetches the IP address of the article's source to help identify its origin and trace potentially malicious sources.

Problem Statement
With the exponential rise of digital platforms and online news, the spread of fake information has become a major challenge globally. Fake news can mislead people, create panic, and influence decisions in domains such as politics, health, finance, and more. The key problem is identifying whether a given piece of news is real or fake, especially when the content appears credible. NewSecure aims to tackle this problem using machine learning and natural language processing techniques.

Objectives
To build a model capable of detecting fake news using supervised learning.

To clean and preprocess news text data to improve model performance.

To implement a feature extraction technique that captures meaningful patterns in the news content.

To evaluate different machine learning models and select the most accurate one.

To enable real-time news article classification using live news feeds.

To display the prediction label along with confidence probability scores.

To retrieve and display the IP address for news predicted as fake to support traceability.

Use Cases
Media platforms can filter and label news content before publishing.

Social media networks can use it to automatically flag suspicious articles.

Educators and researchers can use the tool to study misinformation patterns.

Government and law enforcement agencies can use it for monitoring fake propaganda.

General users can verify the credibility of articles they encounter online.

Technologies Used
The project is implemented using Python and various data science libraries. The primary model used is Random Forest, known for its reliability and interpretability. Natural Language Processing tools are used for text preprocessing, while a vectorization technique like TF-IDF helps convert text into a machine-readable format. News is fetched using the NewsAPI platform, and IP addresses for fake news sources are extracted for traceability.

Model Details
Random Forest was selected after comparing multiple classification algorithms such as Logistic Regression, Naive Bayes, and Decision Tree. Random Forest provided the best accuracy and performance in classifying the textual data. Its ensemble nature allows it to handle noise, irrelevant features, and class imbalance more effectively than other models. Moreover, it can output prediction probabilities, which adds interpretability to the results.

Features
Real vs. Fake classification of news articles based on content.

Cleaned and preprocessed input using standard NLP techniques.

Uses TF-IDF for converting raw text into feature vectors.

Trained using a large dataset of real and fake news samples.

Displays the prediction label with a confidence probability score.

Automatically fetches and classifies live news articles from real-time news feeds using NewsAPI.

If an article is classified as fake, the IP address of its source domain is resolved and displayed.

Advantages
Accurate and interpretable results due to Random Forest's ensemble approach.

Fast and scalable prediction system with real-time capabilities.

Helps raise awareness and counter misinformation online.

Adds a traceability layer by identifying IP addresses of potentially fake sources.

Can be extended to include sentiment analysis, source reliability scoring, or deep learning models.

Limitations
Accuracy may depend on the quality of training data.

NewsAPI may impose rate limits for free-tier usage.

IP address resolution is limited to domains and may not reflect the actual author.

The model may not detect highly sophisticated or contextually manipulated fake news.

Future Work
Integration with a user-friendly web interface for live demo and public use.

Deployment on cloud infrastructure for real-time fake news tracking.

Integration of deep learning models like LSTM, BERT for advanced contextual understanding.

Real-time dashboard for monitoring fake news across categories and geographies.

Feature addition to check historical credibility of sources.

Conclusion
NewSecure offers a reliable and efficient solution to the growing problem of fake news. By combining machine learning with real-time news APIs and traceability features like IP address resolution, this project can contribute meaningfully to the ongoing fight against misinformation. It is a promising foundation for further research and deployment in practical applications.

