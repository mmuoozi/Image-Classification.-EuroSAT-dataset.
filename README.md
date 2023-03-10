# Image-Classification.-EuroSAT-dataset.
Image Classification Task for ML Spacesense Internship 2023



#Constraints of the current solution:

* the biggest limitations of transfer learning is the problem of negative transfer. Transfer learning only works if the initial and target problems are similar enough for the first round of training to be relevant;
* you can not remove layers with confidence to reduce the number of parameters. If you remove the convolutional layers from the first layers, you won't have good learning because of the nature of the architecture which finds low-level features;
* computationally pretty expensive i.e. time-consuming and requires high computational power;
* requires a lot of data;
* training the model from scratch requires a lot of labeled training data and a lot of computing power;
* the number of training data for transfer learning should be in a way that you don’t overfit the model. If you have a few numbers of labeled training data, and your typical pre-trained model, has millions of parameters, you have to be aware of overfitting by choosing appropriate metrics for evaluation and good testing data which represent the real distribution of the real population.


#Potential improvements to the solution:

* one method of improving the performance is fine-tuning. Fine-tuning involves unfreezing some part of the base model and training the entire model again on the whole dataset at a very low learning rate. The low learning rate will increase the performance of the model on the new dataset while preventing overfitting.;
* use another base models and choose the best performing one;
* you  can either download the network weights which saves the time of additional training of the model. Else, we will have to use the network architecture to train our model from scratch;
* the only knowledge we are reusing from the base model is the feature extraction layers. Wecan add another additional layers on top of them to predict the specialized tasks of the model.
