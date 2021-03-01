## Parks and Recreation NLP

### Description
#### The goal of this project is to see how well CorEx topic modeling and Vader sentiment analysis work on Leslie Knope and Ron Swanson's dialogue individually, as well as the conversations between them. 
&nbsp;

### Background
#### Parks and Recreation is a NBC comedy that ran from 2009-2015. It follows the lives of the employees of the Pawnee Parks and Recreation Department. While it has a large ensemble cast, Leslie Knope, the deputy director of the Parks and Recreation Department, is the main protagonist. While she is close to many other characters on the show, she has a particularly unique relationship with her boss Ron Swanson, the director of the Parks and Recreation Department. They have very different views on government and the work of the department, but Leslie views Ron as a mentor and the two are close platonic friends. The project focuses solely on these two characters.
&nbsp;

### Data Used
#### The scripts were obtained from Kaggle - https://www.kaggle.com/heheheluke/parks-and-recreation-scripts
&nbsp;

### Tools Used
#### Data Cleaning, EDA, and Visualization: Glob, Pickle, Pandas, Numpy, Tableau, Re, Matplotlib, WordCloud, Spacy, Seaborn
#### Topic Modeling: Scikit-learn, Nltk, CorEx
#### Sentiment Analysis: vaderSentiment
&nbsp;

### File List
#### 01_Create Data Sets.ipynb - Cleaning the data and creating data sets that will be used for various EDA, visualization, and analysis
#### 02_EDA_and_Word Cloud.ipynb - Calculates number of episodes and show per character and creates wordcloud
#### 03_Corex_Topic_Modeling.ipynb - Code for CorEx topic models for both Leslie and Ron
#### 04_Vader Sentiment Analysis.ipynb - Code for Vader sentiment analysis for Leslie and Ron individually, and the conversations between them
#### 05_Topic Modeling.ipynb - Code for topic modeling done on individual lines and on episodes. This hadn't quite worked as expected so the project pivoted. None of this was included in the presentation, but the code is included here in case it is of interest
#### wordcloud.png - Saved image of the wordcloud used in the presentation
&nbsp;

### Results and Conclusions
#### CorEx topic modeling provided logical results for both characters, but worked better for Ron. The sentiment analysis worked moderately well for the individual characters. Postive sentiment showed a slight upward trend from the beginning to the end of the later seasons, particularly for Ron. The sentiment analysis of the conversations between Leslie and Ron were not that informative. Part of the issue was that the data didn't identify individual scenes, so an approximate method was used for obtaining conversations between Leslie and Ron, which could have missed or counted lines incorrectly. Also, the sentiment analysis sometimes classified certain lines as negative when Ron was trying to help Leslie. I also overlooked the fact that sentiment between two characters is not necessarily the sentiment they feel about one another. 
