In this Folder I have created a model.py file which consists of my Neural Network with 8k Parameters and one Notebook File in which I have Imported the Neural Network
from model.py file to Train it with MNIST Dataset for 20 Epochs. I have trained three models with same Parameters but each one using different Normalisation 
Techniques. I have Elaborated below the Normalisation and the different Normalisation Techniques that i have used for Training the Model, 

Normalization :- 
  It refers to the Process of Shifting and scaling the Input Data such that it has Zero Mean and Standard Deviation. It helps the Network to Maintain smaller Values 
throughout the Network which in turn prevent it from Exploding to a very Big Number. It is done by subtracting Mean from the Input Data and dividing it by standard
Deviation.
  













    
I have named the Three Models that i have trained as Model 1, Model 2 and Model 3. For Model 1, I have used Layer Normalization and for Model 2, I have used
Group Normalization and Batch Normalization along with L1 Regularization has been used for Model 3. From the Results, I have Inferred that Batch Normalization fared better than the other two models followed by Group Normalization and Layer Normalization. For Computer Vision Application, Batch Normalization seems to suit better as we are Normalizing across channels, Similar Features are getting Normalized together. For Natural Language Processing Application, Layer Normalization fares better as sequence of Input Data matters in NLP Application. Hence we need to Normalize all the Channels together for the Input Data. 

                                             Graph I - Validation Loss for all three Models together

![image](https://user-images.githubusercontent.com/61132761/215281122-640e0765-db84-48f1-8fa8-e418b35985d3.png)

                                            Graph II - Validation Accuracy of all Three Model together
                                                  
![image](https://user-images.githubusercontent.com/61132761/215281757-43c9eb49-8c6c-4dc2-ab81-37f769fe8547.png)

I have also shown 10 Misclassified Images for Each Model below, 

i) Model 1 (Layer Normalization) Misclassified Images :- 

![image](https://user-images.githubusercontent.com/61132761/215281834-558436e0-e714-4e25-a42e-eec3bb6ec471.png)

ii) Model 2 (Group Normalization) Misclassified Images :- 

![image](https://user-images.githubusercontent.com/61132761/215281877-af9bc38b-7c61-489b-b13d-bc6bc4576f8e.png)

iii) Model 3 (Batch Normalization with L1 Regularization) Misclassified Images :-

![image](https://user-images.githubusercontent.com/61132761/215281939-41913b92-cd1d-4abc-90f6-616693095c21.png)

