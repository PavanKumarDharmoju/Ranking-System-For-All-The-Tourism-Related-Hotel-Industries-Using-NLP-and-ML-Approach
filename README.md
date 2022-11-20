# Ranking-System-For-All-The-Tourism-Related-Hotel-Industries-Using-NLP-and-ML-Approach
Globally, people witness a booming multi-dollar revenue generation from the hotel industry which increases consistently. This approach is planned to develop a system that ranks different hotel industries worldwide or have a localized ranking for a city or province etc., which considers peoples reviews as its base. Having sufficient number of customers reviews available online help us in this regard. The idea is to analyse the most appreciated tourism related hotel industry to understand the attributes contributing to the revenue. The dataset is acquired from Kaggle which is related to worldwide hotel industries reviews. A novel approach, that uses the ensemble of binary classification called Bidirectional Encoder Representations from Transformers (BERT) model to learn the contextual relations between the words that are necessary for sentence embedding, is implemented. Later, the weighted averages take into account the relative importance and frequency of some factors in our dataset. Using these values, this approach will be able to rank different tourism related hotels. This system can further be enhanced by different stakeholders to plan future ventures based on the results from our model.


We create a model that will be trained to adapt BERT to a hotel review and decide which sentiment radar does the review fall into, either positive, negative or neutral. This method is called fine-tuning.

Later, we train, evaluate and predict the model. We use made-up sentences to evaluate the accuracy of the prediction. For instance, if a positive sentence is entered, the model predicts its sentiment as ‘2’.

In this model, the tokenized input instances are sent into a classifier to convert the example into features. So, these features are sentences, input IDs, tokens, input masks and segment IDs. Later, we load the already pretrained BERT model from the TensorFlow hub and we try to pretrain the model based on our own sentiment task. 

Now, on this model we train, evaluate and finally try to predict a rating for each review given by the user.

Using the test data we take the word count, reviewer score and prediction rating and calculate the weighted average by multiplying the reviewer score with the word count divided by the total number of words
