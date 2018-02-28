---
layout: post
title: Photo Aesthetics Dataset
---

1. The Photo.Net dataset and The DPChallenge dataset 
The Photo.Net dataset contains 20,278 images with at least 10 scores ratings per image. The rating ranges from 0 to 7. 
The DPChallenge dataset contains 16,509 images in total and has been later replaced by the AVA dataset.  You can find some useful information in this [website](http://ritendra.weebly.com/aesthetics-datasets.html). 

2. CUHK-PhotoQuality (CUHK-PQ) dataset
17,690 images collected from DPChallgenge.com and amateur photographers. All images are given the binary aesthetic label and grouped into 7 scene categories: animal, plant, static, architecture, landscape, human and night. The standard training and testing set from this dataset are random partitions of 50-50 split or a 5-fold cross validation partition. The overall ratio of the total number of positive examples and that of the negative examples is around 1: 3. The dataset can be downloaded from [here](http://mmlab.ie.cuhk.edu.hk/archive/CUHKPQ/Dataset.htm). 

3. The Aesthetic Visual Analysis (AVA) dataset
It contains almost 250K images. These images are obtained from DPChallenge.com and labeled by aesthetic scores. Specifically, each image receives 78 ~ 549 votes of score range from 1 to 10. For binary aesthetic quality classification, 5 is used as the threshold. The AVA dataset contains 14 style attributes and more than 60 category attributes for a subset of images. The ratio of the total number of positive examples and that of the negative examples is around 12: 5. You can find the download method [here](https://github.com/mtobeiyf/ava_downloader). 

4. The Image Aesthetic Dataset (IAD)
It contains 1.5 million images derived from DPChallenge and PHOTO.NET. The ratio of the number of positive examples and that of the negative examples is around 1.07: 1.  

5. The Aesthetic and Attributes DataBase (AADB) 
It contains a balanced distribution of professional and consumer photos, with a total of 10,000 images. 11 aesthetic attributes and annotators' ID is provided. 8500 images for training, 500 for validation and 1000 for testing. You can find the download link in their [website](http://www.ics.uci.edu/~skong2/aesthetics.html).

2 and 3 are two standard benchmarks. You can refer to this [survey](https://arxiv.org/pdf/1610.00838.pdf) for more info.
