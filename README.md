# SemiSupervised_learning_Optimization

(Project made together with Erica Marras and Cesare Bidini from the Optimization for Data Science course at UniPd, held by proessor Francesco Rinaldi)

The aim of this project was to address the binary classification problem in a semi-supervised learning scenario, by implementing different gradient descent methods.
Specifically, a limited number of labeled samples and a larger number of unlabeled points have been utilized to develop an accurate model for classifying the correct points labels.

Once defined the loss function, we have implemented the following algorithms:

Gradient Descent with Armijo Rule Line Search
Gradient Descent with Fixed Step-size
Block Coordinate Gradient Descent (BCGD) - Random Rule approach
Block Coordinate Gradient Descent (BCGD) - Gauss-Southwell approach
We utilized a synthetically generated dataset comprising 10,000 points from a bimodal distribution, with each mode representing a separate cluster in the dataset. (Additionally, we evaluated the performance of the model on the challenging "two moons" configuration to optimize the choice of similarity metric and associated parameters.) Then, a random subset of 3% of the points was selected with their true labels, while the remaining points were considered unlabeled.

Furthermore, we have applied the algorithms also for the "Occupancy" real dataset, which includes 6 features (Time, Temperature, Humidity, HumidityRatio, Light, CO2) and a binary target indicating the occupancy status of the office.

We evaluated all the implemented algorithms and conducted a final comparison. The results indicate that the BCGD Gauss-Southwell approach outperfoms the others, achieving an accuracy of 98% for the real dataset.
