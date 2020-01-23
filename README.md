# Web APIs & Classification

### Description

This project is focused on Web Scrapping and Natural Language Processing. Several hundred Reddit posts were pulled from two distinct subreddits. Natural Language Processing was used to analyze the component text of the subreddits in order to create a model that would be able to distinguish which subreddit the post came from based exclusively on the text in each post. The model was created so that any two subreddits could be used.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

### Submission Components

**Natural Language Processing - Reddit.ipynb**: Jupyter Notebook. Contains all code relevent to the project.

**EUROPE_Reddit_Posts.csv**: CSV file. Contains data extracted from Reddit. 
**USA_Reddit_Posts.csv**: CSV file. Contains data extracted from Reddit.

README

Requirements.txt

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

### Problem Statement

Reddit is a website with a tremendous amount of text based data. In order to make it easier to handle, the website is divided into multiple subreddits, which contain posts focused on an individual topic.

The objective of this project is to make it easier to filter out reddit posts into their appropriate subreddits based on the text in the title and body of the posts. 

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

### Methodology 

**Data Extraction**
The initial Web Scrapping of the Reddit website was done using the Reddit PRAW API, which was used to extract multiple data points for each post:

**Extracted Data Points**
- ID
- Title
- Number of Upvotes
- Number of Downvotes
- Subreddit
- Body
- URL
- Number of Comments
- Date Created

**Data Manipulation and Model Construction**

After being extracted, the data was cleaned, standardized, and manipulated in such a way that it could be easily interpreted by Python code and various models.

Several different models and methodologies were experimented with in order to determine the most accurate way of predicting the subreddit of each individual post. 

**Vectorization Methods**
- CountVectorization
- TdifVectorization

**Predictive Models**
- Logistic Regression
- Naive Bayes Classification

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

### Conclusion 

It is possible to predict the source of an individual post with a fair degree of accuracy. In fact, when using the Logistic Regression model, Training data showed a **1.00** average R2-Score, while Testing Data showed a **0.85** average R2-Score.
