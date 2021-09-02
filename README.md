# Fake-News-Detection-System-for-Covid-19

The aim of this project is to create an interpretable model which is trustworthy. When an url is given to the model, along with the output it will also show the reasons on which the following decision was taken, building trust among the use in the system.

What is does ?
1. It takes the URL from the User
2. Extracts the text from the webpage.
3. Send it to the model and predict the outcome. 
4. Later the result is interpreted and the model shows that why it took that decision. 
5. In interpretation, the features are highlighted and weights are given on basis of which the  model prediction was decided. 


What I did ?
1. Created a python script to scrape data from the websites and created a dataset of 37000 articles containing fake and real news. 
2. Choose state of the art attention based model for text classification so that it can understand the context of the words and make better predictions.
3. Created a hybrid deep learning model LSTM-BERT as BERT alone can only take 512 tokens and lenght of average news article was more than 600.
4. Each article was divided into segments of 200 tokens.
5. The BERT Model is then trained over those segments.
6. Pooled output is extracted from those articles and concatenated (articles which have length more than 200 words)
7. Pooled output is then sent to LSTM layer and trained.
8. Later the model was interpreted by LIME model and article was diplayed with highlighted text words along with their words displaying the reasons for the predictions.
9. Finally a research was done on the interpretation of the test result and common patterns and findings was explained.  

