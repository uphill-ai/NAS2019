# Deep Learning for Language Classification

### Joseph Porter, PhD
### Digital Reasoning

Deep learning has revolutionized the application of machine learning to human-relevant tasks.  We will present a tutorial on using basic deep learning techniques to create text classifiers.  We'll discuss the the how and why of deep learning for language, walk through fundamental considerations that affect classifier quality, and discuss the latest approaches.  We'll also provide instructions and data for those that want to follow along and build their own classifiers.

This demo repository contains a Python notebook for creating and running a classification model, and some data.  To get set up, run through the instructions below.  This will involve some software installation and a few commands from your console.

If you have trouble with getting set up ahead of time, please feel free to contact me: 

joseph dot porter@digitalreasoning dot com

Stay tuned to this space for updates -- More interesting things to come!

### Setup (commands to enter are italicized)

Basically, you'll need Python 3 and some data (included here).  You might also need Google Chrome.  Operating system type and version shouldn't matter, as long as you can run a recent version of Python.

You should have a recent processor and at least 8GB of RAM.

1. Install a current Python 3 environment.  We recommend Anaconda: https://www.anaconda.com/distribution/#download-section
1. Google Chrome may also be required.  If your browser has trouble with the instructions below, please install Google Chrome.
1. Download this repository (see the Clone or Download button at the top right for instructions).
1. Create a virtual environment for everything that's necessary (assuming Anaconda):
    1. Open a terminal and navigate to the directory that you downloaded above.
    1. *conda create -n summit python==3.7*
    1. *conda activate summit*
    1. *pip install -r requirements.txt*
    1. *cd bert-sklearn*
    1. *pip install .*
    1. *cd ..*
    1. *jupyter notebook*
1. Open the included notebook file in the browser window that pops up: Competitor-Products.ipynb
1. It will save you time to run most of the notebook once beforehand (more things are downloaded in the background), but that's not strictly necessary.  If you do try it and run into problems, please contact me.

### Files and Directories

bert-sklearn: Copy of the bert-sklearn repository. See above for installation.
data:
* judge-cleaned-up.csv: Twitter Brands and Product Emotions Data
* judge-cleaned-up2.csv: Twitter Brands and Product Emotions Data (preprocessed)
* judge-expanded2.csv: Twitter Brands and Product Emotions, augmented with negatives from Sentiment140 for Apple and Google products, and sampled to reduce neturals to get a balanced data set.
* sent140.zip: Kaggle sentiment 140 data

#### Jupyter Notebooks
Add-Negative Data.ipynb: Create balanced data set from Twitter Brands and Product Emotions data and Sentiment 140.
Competitor-Products-Imbalance-2.ipynb: This is the best starting point for the model - uses balanced data to get a decent classifier.
Competitor-Products-Imbalance.ipynb: Product sentiment classifier exhibiting imbalance issues.
Competitor-Products-Learning Rates.ipynb: Demonstrate slow and fast learning rates
Competitor-Products.ipynb: Original notebook for getting set up and making sure the models are downloaded.
