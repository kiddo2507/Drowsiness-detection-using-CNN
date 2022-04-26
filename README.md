# Drowsiness-detection-using-CNN
Dataset taken from http://mrl.cs.vsb.cz/eyedataset

Once the dataset is downloaded, update the directory's path in ```data_splitting.ipynb```. Once the dataset is splitted into open and close, manually split the data into 90:10 training: testing directories. 

Run the ```model_training.ipynb``` file and change the directory's path of ```/models/model.h5```. Let the model train itself. Personally in my Lenovo Thinkpad T470, i7 processor, 16GB RAM it approximately took 85 minutes to run 5 epoches. 

My model is giving an accuracy of 93.94% after final epoch of 5/5. 

Once the model is trained, go to ```main.ipynb``` file, make necessary changes in the directory path and run the code. It should be working with 
