# Lithofacies_prediction_1-D_CNN
In this notebook we have applied 1-D CNN model to the Force 2020 Lithology prediction dataset

Here's the model summary:
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
-----------------------------------------------------------------
conv1d (Conv1D)              (None, 14, 64)            256       
_________________________________________________________________
batch_normalization (BatchNo (None, 14, 64)            256       
_________________________________________________________________
conv1d_1 (Conv1D)            (None, 12, 64)            12352     
_________________________________________________________________
batch_normalization_1 (Batch (None, 12, 64)            256       
_________________________________________________________________
max_pooling1d (MaxPooling1D) (None, 8, 64)             0         
_________________________________________________________________
batch_normalization_2 (Batch (None, 8, 64)             256       
_________________________________________________________________
conv1d_2 (Conv1D)            (None, 6, 128)            24704     
_________________________________________________________________
batch_normalization_3 (Batch (None, 6, 128)            512       
_________________________________________________________________
conv1d_3 (Conv1D)            (None, 4, 128)            49280     
_________________________________________________________________
batch_normalization_4 (Batch (None, 4, 128)            512       
_________________________________________________________________
max_pooling1d_1 (MaxPooling1 (None, 1, 128)            0         
_________________________________________________________________
batch_normalization_5 (Batch (None, 1, 128)            512       
_________________________________________________________________
flatten (Flatten)            (None, 128)               0         
_________________________________________________________________
dropout (Dropout)            (None, 128)               0         
_________________________________________________________________
dense (Dense)                (None, 64)                8256      
_________________________________________________________________
dropout_1 (Dropout)          (None, 64)                0         
_________________________________________________________________
dense_1 (Dense)              (None, 32)                2080      
_________________________________________________________________
dropout_2 (Dropout)          (None, 32)                0         
_________________________________________________________________
dense_2 (Dense)              (None, 16)                528       
_________________________________________________________________
dense_3 (Dense)              (None, 12)                204       

Total params: 99,964
Trainable params: 98,812
Non-trainable params: 1,152
_________________________________________________________________

Training data can be downloaded from the link given below:

https://github.com/bolgebrygg/Force-2020-Machine-Learning-competition/tree/master/lithology_competition/data
