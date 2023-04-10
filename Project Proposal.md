**Developing a Sentiment Analysis Model** 




**Reference Project link :**

<https://www.kaggle.com/code/shreyasingh235/real-time-data-sentiment-analysis>

**Dataset link :**

<https://www.kaggle.com/datasets/ilhamfp31/yelp-review-dataset>




**Introduction**

Sentiment Analysis has an important role in today’s world especially for private companies which hold lots of data. In this project proposal, we will describe how a sentiment analysis Model has been developed to provide real-time sentiment analysis. The team will be responsible for developing the model and training it on different dataset using the algorithms Bert and CNN.

**Background**

We took the reference of a pre-existing project on sentiment analysis of tweets, used its model training techniques of BERT-CNN-BiLSTM learning pipeline, which consists of three sequential modules. We went through it’s tweet dataset and results which consisted of binary polarity and elapsed time for it.

**Project Objective**

The primary objective of the project is to develop a Model that can perform real-time sentiment analysis for businesses to quickly respond to customer feedback and improve customer satisfaction.  The following are some of the specific objectives of the project:

- Train the model using a large and diverse customer review dataset to ensure it can handle different types of language, styles, and domains.
- Implement the model as a tool for businesses to monitor customer feedback and sentiment across various channels, such as social media, online reviews, and customer service interactions.
- Conduct extensive testing and evaluation of the model's performance, including metrics such as accuracy, precision, recall, and F1-score, to ensure it can provide reliable and actionable insights for businesses.


**Enhancements**

- Another Yelp review dataset is used instead of tweets data.
- Calculating the polarity of reviews using VADER
- VADER produces four different types of classes : negative, neutral, positive, compound
- Train the model on training dataset using BERT-CNN-BiLSTM (the similar techniques of shared project link but on a different dataset)
- Evaluating and Improving overall accuracy
- Integration of a chatbot for real time input analysis of reviews done by customer.





**Methodology**

**Dataset :** 

The Yelp reviews dataset consists of reviews from Yelp.The Yelp reviews polarity dataset is constructed by considering stars 1 and 2 negative, and 3 and 4 positive. For each polarity 280,000 training samples and 19,000 testing samples are take randomly. In total there are 560,000 trainig samples and 38,000 testing samples. Negative polarity is class 1, and positive class 2.

**Text Pre-processing :**

Remove urls, html tags and punctuations, Using NLTK libraries 

**Polarity and Intensity Calculation** :

Using Vader library provided by NLTK to produce four different types of classes : negative, neutral, positive, compound.

**Mapping Target level to String** :

Mapping the labels [0:Bad, 1:negative,2:neutral, 3:positive,4:great] to the review text.

**Model Training** :

` `BERT-CNN-BiLSTM learning pipeline, which consists of three sequential modules.

- BERT is utilized to transform word tokens from the raw Tweet messages to contextual word embeddings.
- CNN is known for its ability to extract as many features as possible from the text.
- BiLSTM keeps the chronological order between words in a document, thus it has the ability to ignore unnecessary words using the delete gate.

**Chatbot Integeration** :

We will be building a real time chatbot out of it using platforms of NLP/frameworks and the chatbot's response can be defined based on the sentiment, for example, a positive sentiment score will trigger a happy response, while a negative sentiment will trigger a response that offers assistance or empathy. 

**Conclusion**

The project proposal aims to develop a sentiment analysis model for real-time analysis of customer reviews and integrating a chatbot for businesses to monitor customer feedback and sentiment across various channels. The proposed enhancements include using the Yelp reviews dataset, calculating polarity using VADER, and improving overall accuracy.

The methodology involves data pre-processing, polarity and intensity calculation, and model training using BERT-CNN-BiLSTM. The chatbot will provide responses based on the sentiment score, offering responses based on the sentiments. The project's success will be evaluated based on metrics such as accuracy, precision, recall, and F1-score to ensure reliable and actionable insights for businesses.
