# Food_Image_Query
Just a rapid proof-of-concept (5 hrs) for my app and practice\
Downsize the database for idea testing. The data is from Food Images (Food-101). You can download it from https://www.kaggle.com/datasets/kmader/food41

# Steps:
1. Use Resnet18 as feature selection 
2. The features are then treated as vector 
3. Find the clustering based on cosine distance 

Assume the user upload this picture into our database:
<img width="184" alt="image" src="https://user-images.githubusercontent.com/45325095/166091220-20990a77-c1ab-47de-9fa8-82112f9ad778.png">

Our system should be able to roll out similar pictures that the other uses took (already in the database)
<img width="248" alt="image" src="https://user-images.githubusercontent.com/45325095/166091238-71b75983-1bb9-4e3d-8060-6fbbb2446190.png">


# Upcoming Future Work:
1. Need to cut the image center (too much distraction atm)
2. Need to do some sensitivty analysis on the tree for Annoy :) 
3. Test out how it will be with a more sophisticated feature selector (Resnet50!) 
4. Train the classification system just for the completeness
5. Of course, nicer pictures (better lighting/ contrast/ more center) will definitely helps 

# Reference
1. Food-101 Database from Kaggle https://www.kaggle.com/datasets/kmader/food41
2. https://github.com/spotify/annoy
3. K. He, X. Zhang, S. Ren, and J. Sin. Deep Residual Learning for Image Recognition. 2015
