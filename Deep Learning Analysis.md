# Deep Learning Analysis

# Data Processing and Results
In the first test, EIN and NAME were dropped from the dataset and the remaining columns were considered features for the model. THe data was split into training and testing sets of data where the target variable "IS_SUCCESSFUL" is verified by the value 1 and 0 being not successful. APPLICATION data was analyzed, and CLASSIFICATION's value was used for binning.

Neural Network was applied on each model with 3 layers total, which only had an accuracy about 73%.
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense (Dense)               (None, 7)                 350       
                                                                 
 dense_1 (Dense)             (None, 14)                112       
                                                                 
 dense_2 (Dense)             (None, 1)                 15        
                                                                 
=================================================================
Total params: 477
Trainable params: 477
Non-trainable params: 0
_________________________________________________________________

268/268 - 0s - loss: 0.5511 - accuracy: 0.7338 - 256ms/epoch - 954us/step
Loss: 0.5511336326599121, Accuracy: 0.7337609529495239

In the second test, NAME was added back in the dataset which gained a higher accuracy of about 79%.

Model: "sequential_1"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense (Dense)               (None, 7)                 3171      
                                                                 
 dense_1 (Dense)             (None, 14)                112       
                                                                 
 dense_2 (Dense)             (None, 1)                 15        
                                                                 
=================================================================
Total params: 3,298
Trainable params: 3,298
Non-trainable params: 0
_________________________________________________________________

268/268 - 0s - loss: 0.4797 - accuracy: 0.7890 - 202ms/epoch - 753us/step
Loss: 0.4797488749027252, Accuracy: 0.7890378832817078

Deep learning models should have multiple layers since it is machine based so that computers can filter inputs through the layers to learn how to predict and classiy information that it is given.