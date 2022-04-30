# Food_Image_Query
Just a rapid proof-of-concept (5 hrs) for my app and practice\
Downsize the database for idea testing. The data is from Food Images (Food-101). You can download it from https://www.kaggle.com/datasets/kmader/food41

# Steps:
1. Use Resnet18 as feature selection 
2. The features are then treated as vector 
3. Find the clustering based on cosine distance 

# Expected Behavior:
Assuming the user upload this picture into our database:\
![image](https://user-images.githubusercontent.com/45325095/166091347-ece9690b-8a49-43d6-8f4f-b20d07a552a3.png)

Our system should be able to roll out similar pictures that the other uses took (already in the database)\
![image](https://user-images.githubusercontent.com/45325095/166092424-6bbdbef7-b50c-4f39-b2e8-162bf4fc25e7.png)


# Upcoming Future Work:
Of course, this rapid preliminary version is not getting perfect results as you can see from the notebook.\
Currently, the system is doing quite well for french fries, fried rice, and donuts. I will probably spend some time either getting better picture from webscrapping or clean the image dataset more. Along with that, several more adjustments will be made:
1. Need to cut the image center (too much distraction atm)
2. Need to do some sensitivty analysis on the tree for Annoy :) 
3. Test out how it will be with a more sophisticated feature selector (Resnet50!) 
4. Train the classification system just for the completeness
5. Of course, nicer pictures (better lighting/ contrast/ more center) will definitely helps 

# Reference
1. Food-101 Database from Kaggle https://www.kaggle.com/datasets/kmader/food41
2. https://github.com/spotify/annoy
3. K. He, X. Zhang, S. Ren, and J. Sin. Deep Residual Learning for Image Recognition. 2015
