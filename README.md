# Deep Learning Homework Report

## Data Preprocessing

* What variable(s) are considered the target(s) for your model?
	* APPLICATION_TYPE
	* AFFILIATION
	* CLASSIFICATION
	* USE_CASE
	* ORGANIZATION
	* STATUS
	* INCOME_AMT
	* SPECIAL_CONSIDERATIONS
	* ASK_AMT
* What variable(s) are considered to be the features for your model?
	* IS_SUCCESSFUL

* What variable(s) are neither targets nor features, and should be removed from the input data?
	* NAME / EIN
	* ASK_AMT was removed from my input data because I thought it would improve the accuracy and had a quasi-proxy in the binned "Income_Amt"

## Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
	* I used two hidden layers (relu) with 80 / 25 neurons and an output layer (sigmoid).
	* I used this to simply match the provided sample code. My knowledge of this topic is not strong enough to provide a more developed answer.
* Were you able to achieve the target model performance?
	* NO, my attempts got close with around 74%
* What steps did you take to try and increase model performance?
	* I attempted to reduce the noisiness of the data by removing the ASK_AMT column
	* I attemped to double the epochs, wrongly assuming that my accuracy hadn't quite leveld out at 100 epochs
	* I attempted to add layers, modify the neurons and split the difference on the epochs at 150

## Summary:

* overall results of the deep learning model.
	* Overall the results of the model were not at the desired accuracyb but they were close.
	* A closer inspection of the different features could have reduced noisiness further, but overall it was fine.
* Different model recommendation:
	* After researching the different use cases for NN models, I would probably stick with the sequential model
	* CNN are mostly for image related tasks and RNNs could maybe fit, but I'm not sure
	* I would say that further tinkering with the existing sequential model would be the optimal way to tackle this use case