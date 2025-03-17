# deep-learning-challenge
Alphabet Soup Deep Learning Model Report
Overview of the Analysis
The goal of this analysis is to evaluate the performance of a deep learning model designed to classify companies' success or failure based on various features in the Alphabet Soup dataset. By applying a neural network, we can learn the underlying patterns and relationships between these features and the target variable, providing a foundation for future improvements in prediction accuracy.
Results
Data Preprocessing
•	Target Variables: 
o	The target variable for this model is the "success" label, which indicates whether a company is successful (1) or not (0).
•	Feature Variables: 
o	The features used in the model include the financial and performance-
Compiling, Training, and Evaluating the Model
•	Neurons, Layers, and Activation Functions:
o	Neurons and Layers: 
	The model includes six layers in total: 
	First hidden layer: 110 neurons
	Second hidden layer: 80 neurons
	Third hidden layer: 60 neurons
	Fourth hidden layer: 70 neurons
	Fifth hidden layer: 115 neurons
	Sixth hidden layer: 90 neurons
	Activation Functions: 
	The ReLU activation function is used in the hidden layers to introduce non-linearity and allow the network to learn more complex patterns.
	The sigmoid activation function is used in the output layer, which is suitable for binary classification (predicting success/failure).
•	Achieving Target Performance:
o	The model was able to train and evaluate with reasonable accuracy, but did not achieve a high enough target performance after 100 epochs of training.
o	Training Accuracy: The model achieved a satisfactory training accuracy but exhibited some overfitting, as seen in validation accuracy during training.
•	Steps Taken to Increase Model Performance:
o	Dropout Layer: A dropout layer with a rate of 50% was added after the hidden layers to mitigate overfitting and improve generalization.
o	Early Stopping: Implemented early stopping to halt training once validation loss no longer improved for 10 consecutive epochs.
o	Learning Rate Optimization: The Adam optimizer was used with a learning rate of 0.001, but further tuning may be necessary for better performance.
o	Model Architecture Adjustments: Experimented with adjusting the number of layers and neurons per layer, but further refinement may be needed.
Summary
•	Overall Results: 
o	Adding additional layers and tweaking hyperparameters (e.g., batch size, learning rate) might lead to better performance, but the current configuration still shows promising results.
•	Recommendation for Future Models: 
o	Additional Data Engineering: Further feature engineering, such as creating new interaction terms or aggregating features, could enhance model accuracy.

