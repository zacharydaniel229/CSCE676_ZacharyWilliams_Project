# Amazon sales and reviews dataset analysis

My project is an analysis of an amazon product dataset. This dataset includes information about the project such as price, discount, and category as well as ratings and reviews for the product. I analyzed whether or not features like discounts or the category affected the rating. I also generated text embeddings from the reviews and clustered them. 

# Main Notebook

The main notebook is [Link text](main_notebook.ipynb).

# Research Questions

I chose to ask two questions that are tightly connected because I wanted to explore both reviews and ratings which are two different methods of evaluating a product. These questions were “Are the ratings biased by the category or discounted amount?” and “What clusters emerge from review text embeddings?”

# Project video

https://youtu.be/95UwwN8um9Q

# Dataset Selection

I chose an amazon products dataset that includes basic information about the product as well as a review and rating for the product. Each product belonged to a category. Over 95% of the products were a part of one of three main categories, Computer and accessories, electronics, or home and kitchen.

# Reproducing work.

This was built locally in VsCode. The requirements to duplicate the environment is in [Link text](requirements.txt). To install the requirements, run the command, "pip install -r requirements.txt". To run the notebooks in chronological order, run checkpoint_1.ipynb, checkpoint_2.ipynb, and then main_notebook.ipynb.

# Key dependencies.

Although the recommend way to run the code is to create an environment with the dependencies in requirements.txt, the main dependencies are python 12.2, scikit-learn==1.8.0, torch==2.11.0, pandas==2.3.3, notebook==7.5.2, numpy==2.4.1, matplotlib==3.10.8.

# Repo structure.

All of the files live in the root directory. This directory includes the three python notebooks, the requirements file, and the README file.

# Results summary.

I did multiple tests to determine if the category affected the rating. I found that the computers and accessories category significantly affected the rating, but I did not find any evidence of a difference between electronics and home and kitchen. The word2vec embeddings made 2 clusters with large majorities as computers and accessories and another with a large majority as electronics and home and kitchen. This is just like earlier when the models could not differentiate ratings based on these two categories. On the other hand, BERT embeddings gave each category its own cluster.