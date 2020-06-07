# [Project 1 : Signal-Classification](https://github.com/omrigo5/Signal-Classification)
This work was prepared as a final project of a course I completed in the Weizmann Institute of Science during my PhD studies. Course name: "Practical Deep Learning for Science" by Prof. Eilam Gross
Goal: demonstrate remote optical eavesdroping. 
For example, record a meeting which takes place in an isolated building by record the vibrations of the windows (or any other nearby object) and reconstruct the audio signal. 
There are numerous challeges in executing this goal:
Audio frequencies varies between 20 Hz to 20,000 Hz that requires very Fast sampling rate ( 20,000 Hz signal corresponds to sampling of 50μs) with "Tons" of data to record
Probably low SNR (Signal to Noise ratio)
An unknown transmission of the window and setup
![](https://github.com/omrigo5/Signal-Classification/blob/master/objective.jpg?raw=true)

# [Project 2 : Hotel-Booking-Cancellation](https://github.com/omrigo5/Hotel-Booking-Cancellation)
Goal : Predict the chances of cancelation using data of costumers from multiple hotels. The data is given in a tabular form of 32 columns (20 numerical + 12 objects), and taken from Kaggle datasets: https://www.kaggle.com/jessemostipak/hotel-booking-demand
As a first stage the data was seperated to training/validation/test sets. To get the optimal model I have investigated the features in the training-set, starting with the numerical features that are most correlated with the target. I proceded with encoding the categorical features while monitoring the accuracy with a small subset of features to get an initial estimation of the achievable prediction.
Model selection was made by considering three models (Random Forest, Gradient Boosting and Logistic Regression) and evaluating them on the validation set. The effectiveness of dimensionality-reduction (using PCA) and model tuning (using Grid-Search) was assessed as well.
![](https://github.com/omrigo5/OG-Portfolio/blob/master/Images/scores%20of%20models.png?raw=true)
