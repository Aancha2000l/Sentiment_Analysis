# Sentiment_Analysis
Sentiment Analysis is a process of extracting opinions with varried polarities. Plarities mean positive, negative or neutral. It is a type of classification where data is classified into different classes. WHere these classes can be binary as in positive or negative or can have multiple classes. With the help of Sentiment Analysis , We can find the nature of opinion reflected in the text, document , website or feed etc.

Our model is Binary classification model which tells postive or negative based upon the emotion displayed by the dataset. Dataset is a webscrapped data from a news site named as inshorts using BeautifulSoup library from bs4 which is extracted in form of headline article and category such as sports , politics , etc.

Once, The dataset is available preprocessing is done in order to clean the data. With the help of nltk which is Natural Language Tool Kit stopwords are loaded , These stop words are like an, the , a , in ,i etc which are removed from the dataset for saving valuable processing time. All the unnessesary html tags are removed from the dataset, special characters are removed, any kind of contractions or abbrevations are expanded witht the help of contraction library.

After Cleaning of dataset , we extract the required information by using SentimentIntensityAalyzer from vadersentiment the polarities of the data is checked. The positive value tells about positve sentiments and vice versa . The required prediction column containing postivie and negative is created with the help of polarities. unnecessary Columns are dropped and a clean and required dataset is available for use.

Once we obtain a clean dataset the next step is to build our model.
