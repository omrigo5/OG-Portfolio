Description of my data-science projects with links to their GitHub repositories:
# [Project 1 : Signal-Classification](https://github.com/omrigo5/Signal-Classification)
This work was prepared as a final project of a course I completed in the Weizmann Institute of Science during my PhD studies.
("Practical Deep Learning for Science" by Prof. Eilam Gross)  
Goal: demonstrate remote optical eavesdroping.  
For example, record a meeting which takes place in an isolated building by record the vibrations of the windows (or any other nearby object) and reconstruct the audio signal.  
Sampling was carried out by an optical setup; a laser beam was reflected from a mirror that was attached to a speaker, the vibrations of the mirror served as the translation of the acoustic signal to an optical one. The optical signal was processed by a Lock-in amplifier which amplifies pre-defined frequencies with high SNR. As the the sampling rate was low (and shrunk even further while preprocessing the data) and the transmission function of the mirror was unknown, the audio was impossible to reconstruct in any analytical method.  
The training was performed on slices of sequenced data with the audio source as a target label. The model was prepared as a classification model for the sequenced data. Two approaches were examined:
* RNN (lstm) - a natural choice for time-series data where the order of the data is meaningful
* one-dimensional CNN - an adaptation of convolution that usualy used in 2D and 3D for image analysis to detect patterns in 1D
![](https://github.com/omrigo5/Signal-Classification/blob/master/objective.jpg?raw=true)


# [Project 2 : Hotel-Booking-Cancellation](https://github.com/omrigo5/Hotel-Booking-Cancellation)
Goal : Predict the chances of cancelation using data of costumers from multiple hotels. The data is given in a tabular form of 32 columns (20 numerical + 12 objects), and taken from Kaggle datasets: [kaggle.com/jessemostipak/hotel-booking-demand](https://www.kaggle.com/jessemostipak/hotel-booking-demand)  
As a first stage the data was seperated to training/validation/test sets. To get the optimal model I have investigated the features in the training-set, starting with the numerical features that are most correlated with the target. I proceded with encoding the categorical features while monitoring the accuracy with a small subset of features to get an initial estimation of the achievable prediction.  
Model selection was made by considering three models (Random Forest, Gradient Boosting and Logistic Regression) and evaluating them on the validation set. The effectiveness of dimensionality-reduction (using PCA) and model tuning (using Grid-Search) was assessed as well. 
![](https://github.com/omrigo5/Portfolio-Omri-Goldberg/blob/master/Images/combined.png?raw=true)  
