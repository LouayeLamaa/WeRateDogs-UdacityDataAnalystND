# WeRateDogs Twitter Analysis
## Project Overview

WeRateDogs is a Twitter account that posts and rates pictures of dogs. These ratings often are not serious and have numerators that are greater than the denominators. The goal of this analysis is the wrangling of WeRateDogs's Twitter archive to create intresting analyses and visualizations. 

In this project, I worked on three datasets:

### 1- Enhanced Twitter Archive:

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, I have filtered for tweets with ratings only (there are 2356). This data is given by Udacity

### 2- Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. I gathered this data from Twitter's API using Tweepy.

### 3- Image Predictions File

Udacity ran the images on WeRateDogs's account through a neural network to generate three predictions for each image. The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images). This file was downlaoded programmatically using requests library.
