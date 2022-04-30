# Food_Image_Query
Just a rapid proof-of-concept (5 hrs) for my app and practice\
Downsize the database for idea testing. The data is from Food Images (Food-101). You can download it from https://www.kaggle.com/datasets/kmader/food41

# Steps:
1. Use Resnet18 as feature selection 
2. The features are then treated as vector 
3. Find the clustering based on cosine distance 




# Upcoming Future Work:
1. Need to cut the image center (too much distraction atm)
2. Need to do some sensitivty analysis on the tree for Annoy :) 
3. Test out how it will be with a more sophisticated feature selector (Resnet50!) 
4. Train the classification system just for the completeness 

# Reference
1. https://github.com/spotify/annoy
2. K. He, X. Zhang, S. Ren, and J. Sin. Deep Residual Learning for Image Recognition. 2015
