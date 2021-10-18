# Portfolio
---

## Table of Contents
* [Reddit Mini Project](#redditminiproject)

---

### Identifying Reddit Topics Using K-Means<a name="redditminiproject"></a>

#### Keywords
* clustering, unsupervised machine learning
* vectorization, tf-idf
* dimensionality reduction, tsvd
* data visualization and storytelling

#### Project Summary
Reddit is an online discussion site, where people come together to bring up and discuss about various topics. The objective of this project was to identify the topics present in a sample of about 6000 reddit posts.

The data was preprocessed by cleaning and removal of duplicated entries, and the frequently-appearing terms in the post titles were identified in order to get preliminary insights as to what the topics might be.

Clustering was performed on the the clean post titles. First, the post titles were vectorized using TF-IDF. After that, the dimensionality of the vectors was reduced using TSVD. The criterion for dimensionality reduction was that the cumulative variance explained needed to be at least 80%. K-Means clustering was then performed and the optimum number(s) of clusters was taken based on internal validation criteria. The clusters formed were interpreted in an attempt to identify the topic of each.

#### Links
* [Write-Up](/html_previews/redditminiproject/redditminiproject.html)
* [Project repository on github](https://github.com/oonrezak/reddit_mini_project)

---
[Project 2 Title](/pdf/sample_presentation.pdf)
<img src="images/dummy_thumbnail.jpg?raw=true"/>

---
[Project 3 Title](http://example.com/)
<img src="images/dummy_thumbnail.jpg?raw=true"/>

---

### Category Name 2

- [Project 1 Title](http://example.com/)
- [Project 2 Title](http://example.com/)
- [Project 3 Title](http://example.com/)
- [Project 4 Title](http://example.com/)
- [Project 5 Title](http://example.com/)

---




---
<p style="font-size:11px">Page template forked from <a href="https://github.com/evanca/quick-portfolio">evanca</a></p>
<!-- Remove above link if you don't want to attibute -->
