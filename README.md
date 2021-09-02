# Fake-News-Detection-System-for-Covid-19

The aim of this project is to create an interpretable model which is trustworthy. When an url is given to the model, along with the output it will also show the reasons on which the following decision was taken, building trust among the use in the system.
Training: 
1. Scraped data from the websites to create a dataset of 37000 articles containing fake and real news. 
2. The articles are divided into segments if its length is more than 200 words as BERT can only take 512 tokens.
4. The BERT Model is then trained over those segments.
5. Pooled output is extracted from those articles and concatenated (articles which have length more than 200 words)
6. Pooled output is then sent to LSTM layer and trained.

What is does ?
1. It takes the URL from the User
2. Extracts the text from the webpage.
3. Send it to the model and predict the outcome. 
4. Later the result is interpreted and the model shows that why it took that decision. 
5. In interpretation, the features are highlighted and weights are given on basis of which the  model prediction was decided. 
