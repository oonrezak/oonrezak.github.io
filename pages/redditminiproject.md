## Identifying Reddit Topics Using K-Means

<div class="gridwrapper">
  <div class="one"><img src="../images/redditminiproject/dim_redux_1.jpg?raw=true"/></div>
  <div class="two"><img src="../images/redditminiproject/clustering_1.jpg?raw=true"/></div>
  <div class="three"><img src="../images/redditminiproject/internal_val_1.jpg?raw=true"/></div>
  <div class="four"><img src="../images/redditminiproject/reddit_wordcloud_1.jpg?raw=true"/></div>
</div>

<br />
### Keywords
* clustering, unsupervised machine learning
* vectorization, tf-idf
* dimensionality reduction, tsvd
* visualization, storytelling

### Project Summary
Reddit is an online discussion site, where people come together to bring up and discuss about various topics. The objective of this project was to identify the topics present in a sample of about 6000 reddit posts.

The data was preprocessed by cleaning and removal of duplicated entries, and the frequently-appearing terms in the post titles were identified in order to get preliminary insights as to what the topics might be.

Clustering was performed on the the clean post titles. First, the post titles were vectorized using TF-IDF. After that, the dimensionality of the vectors was reduced using TSVD. The criterion for dimensionality reduction was that the cumulative variance explained needed to be at least 80%. K-Means clustering was then performed and the optimum number(s) of clusters was taken based on internal validation criteria. The clusters formed were interpreted in an attempt to identify the topic of each.

### Links
* [Notebook and Write-Up](/html_previews/redditminiproject/redditminiproject.html)
* [Project repository on github](https://github.com/oonrezak/reddit_mini_project)
* [Back to Main Page](https://oonrezak.github.io/)