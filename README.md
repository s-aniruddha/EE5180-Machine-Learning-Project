## Using summaries to improve sentiment classification

This is a project I submitted towards the group project in the course EE5180 Introduction to Machine Learning @ IIT Madras. In this project, I use a novel method for review sentiment classification based on Hierarchical classification, review text, and the summary. The model has far fewer trainable parameters than the state-of-the-art in 2020 and yet achieves competitive performance.

### Model Description

First, a BiGRU based model will classify whether a review is positive (4-5 rating) or negative (1-3 rating) using the short summary text of the review. Then based on whether a review is classified positive or negartive by the first stage classifier, another BiGRU based model will use the full summary text to perform finer classfication and generate the prediction rating. The model is tested on the Sports and Outdoors dataset from Amazon 5 cores repository, which has the review text, rating and the review summary text. The dataset can be found in [this page](https://nijianmo.github.io/amazon/index.html).
