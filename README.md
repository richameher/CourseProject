# CourseProject

### Presentation and Tutorial Available at - https://mediaspace.illinois.edu/media/t/1_ammbs24f?st=0

### Code folder contains 

1. Final Project V4.ipynb  (whole source code)
2. Test.ipynb (Code for testers to run)
3. requirements.txt (libraries to install)
4. sentiment_analyzer.joblib (trained sentiment classifier model)

### Data Folder contains 

1. preprocess_airbnb.csv (Airbnb data with necesaary n-grams extracted with source code  to be used for topic extraction and sentiment analysis)
2. preprocess_hotel.csv (Hotel data with necesaary n-grams to be used for topic extraction and sentiment analysis)

### Complete documentation available in 
Project Documentation.pdf

### You can view my ipynb notebooks directly using nbviewer
https://nbviewer.jupyter.org/github/richameher/CourseProject/blob/main/code/Final_proj%20V4.html

### Software Implementation and Usage

#### 1. (Optional) Create a Python3 virtual environment

```python3 -m venv py3-env-final-proj```

#### 2. (Optional) Activate virtual environment

```source py3-env-final-proj/bin/activate``` 

#### 3. 

```pip install jupyter```

#### 4. Install ipykernel in this environment-  

```python3 -m ipykernel install --user —name=final-proj```
 
 (final-proj will be used as env in jupter notebook)

#### 5. 

```pip install -r requirements.txt```

#### 6. Start Jupyter-notebook from shell using command :  

```jupyter notebook```

#### 7. Download this github repository and open the Test.ipynb file 

#### 8. Switch to final-proj kernel defined in step 4.

#### 9. Change the file path to where the preprocessed files are i.e. under folder data and Run all the cells in the notebook

### Methodology (Code in code/Final Project V4.ipynb)

1. Read Original Datasets (Check Proposal.pdf Data for the links)
2. Clean Text- Tokenize, Remove punctuations, tabs, whitespaces, stopwords, common words
3. Extract bigrams- Create a bigrams column to extract all afjacent pairs of bigrams from review/text
4. Create a bigram_list column and keep bigrams that are NN-ADJ pairs
5. Create a unigram_list column and keep only unigrams that are NN
6. Train a Logistic Regression classifier on sentiment and reviews of the hotel dataset as only 
hotel dataset has ratings (map ratings to sentiments first)
7. Use WordCloud to visualize frequent bigrams
8. Use TF-IDF to extract top n keywords from unigrams or bigrams
9. Use the trained sentiment classifier to classify the sentiment for the keywords
10. Plot a bar graph, with sentiment as labels, keywords and sentiment probability/topic extent on Y-axis

### Results 

[Hotel Review Bigram WordCloud]

![alt text](https://github.com/richameher/CourseProject/blob/main/images/hotel_review_wordcloud.png)

[Hotel Review Sentiment-Topic Extent Bar Plot]

![alt text](https://github.com/richameher/CourseProject/blob/main/images/Hotel_Aspectsentiment.png)

In the Wordcloud we can observe that people tend to talk about the quality of rooms. Features like safety is usually associated with the hotels than Airbnbs. Also Hotels have their own website , so people also talk about the online booking system. As for the bar plot, we can see that hotels have “theft”, “suite” aspects that have been associated with negative sentiment. Also the highest positive sentiment is observed among aspects like “room”, “view” and “manager” 

##### (Note- we can also observe the sentiment probability on y-axis instead of topic extent, Check Test.ipynb)

### Contribution

Completed By Richa Meherwal 

Free Topic- Using Topic Mining and Sentiment Analysis to compare customer level satisfaction in Airbnb vs Hotels
