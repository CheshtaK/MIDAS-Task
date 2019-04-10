# CV_problem
**Problem Statement**: This dataset has 4 classes. Labels for training data are provided, you have to submit labels of test data. 
Feel free to use any Machine learning or Deep learning technique.

## Evaluation Procedure
I split the training data randomly into train (75%) and test (15%). The test dataset of 2000 images are used for final evaluation. 
I created two models - one without adding checkpoints and the other as the best model with checkpoints. Finally I used the best model
to make predictions for the test dataset.

## Results
For my first simple CNN model with basic layers, there are 143,876 trainable parameters. The model summary is as follows:

![alt-text](https://github.com/CheshtaK/Task/blob/master/root/CV_problem/model_summary.PNG)

The model accuracy is around 86.67%.

* Plots illustrating the accuracy/loss of training and validation over time:

![alt-text](https://github.com/CheshtaK/Task/blob/master/root/CV_problem/model_plots.PNG)

For my second deeper model (my_model.h5), I added more layers which resulted in a total of 345,926 trainable parameters. The model summary is as follows:

![alt-text](https://github.com/CheshtaK/Task/blob/master/root/CV_problem/improved_model_summary.PNG)

The model accuracy is around 88.5%.


* Plots illustrating the accuracy/loss of training and validation over time:

![alt-text](https://github.com/CheshtaK/Task/blob/master/root/CV_problem/improved_model_plots.PNG)


## Conclusion
The final best model (best_model.h5) is saved after adding checkpoints so as to overcome the problem of overfitting. The given test dataset is then evaluated using this model and the predictions are stored in a .csv file.
