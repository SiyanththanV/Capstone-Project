
# Capstone Project
Objective of capstone project was to find like-minded users grouped as communities. Tweets from Twitter was used for the purpose of this project, to detect topics and build user communities of users who share similar interests in these topics. 

### Topic Detection-Latent Dirichlet Allocation (LDA)
LDA modelling was used to detect topics based on the pre-processed content posted by users in their tweets. LDA modelling depends on probabilistic calculation to find the most relevant topics. Each document is a distribution of topics and each topic was a distribution of words.

### Community Detection
Each user that was accounted for in the aggregation of tweets was represented as a k-dimensional vector, where k was the number of topics assigned for LDA topic detection. Each user vector indicated how relevant a topic was to a given user for all the topics detected by LDA analysis. User vectors were then used as inputs for K-means clustering to form a given set of clusters of users who shared similar interests in topics. The resulting clusters or communities of users showed users who were like-minded and had similar interests based on their social media content.

### Evaluation Method
The algorithm's performance was evaluated and measured by applying the algorithm in two applications; user recommendation and user predication systems. User recommendation consisted of recommending the most relevant content to users based on the history of their posted content and interests. User prediction consisted of predicting which user may have posted a specific content and measure the degree of prediction accuracy. As such, both these applications led to the following evaluation metrics; S@K, MRR, precision, recall and F-Measure.

## Technologies
- Python and Jupyter notebooks for cell-based execution
- Python's Gensim package for LDA topic modelling 
- Python's scikit-learn package for k-means clustering and cosine similarity calculation
- Google Cloud Platform development tools:
	- Compute Engine VM instances for high volume and extensive execution
	- Cloud Storage for file management on VM instances
	- BigQuery for querying large Twitter datasets

## Repo Contents
This repo consists of the Python notebooks with the methodology and approach investigated, implemented and evaluated in this capstone project. It consists of the resulting LDA and k-means models for various number of topics and clusters for benchmarking and evaluation purposes. 
