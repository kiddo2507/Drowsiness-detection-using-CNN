# Drowsiness-detection-using-CNN
Dataset taken from http://mrl.cs.vsb.cz/eyedataset

Once the dataset is downloaded, update the directory's path in ```data_splitting.ipynb```. Once the dataset is splitted into open and close, manually split the data into 90:10 training: testing directories. 

Run the ```model_training.ipynb``` file and change the directory's path of ```/models/model.h5```. Let the model train itself. Personally in my Lenovo Thinkpad T470, i7 processor, 16GB RAM it approximately took 85 minutes to run 5 epoches. 

My model is giving an accuracy of 93.94% after final epoch of 5/5. 

Average of accuracy for all the epochs, i.e., the accuracy of the InceptionV3 model is 93.294% and the final loss of the model came out to be 18.11%.

I even tried using ResNet50 for training the model and The average accuracy and loss after using ResNet50 neural network architecture was 50.484% and 69.312% respectively. You can see this work in ```resnet_model_training.ipynb``` file and see all the layers of it in ```resnet_output.txt```.

Once the model is trained, go to ```main.ipynb``` file, make necessary changes in the directory path and run the code. It should be working with 
