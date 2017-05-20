[image1]: ./imgs/result.png

## Сeleraone-Test-Solution

---

## Task

The file task_data.csv contains an example data set that has been artificially generated. 
The set consists of **400** samples where for each sample there are **10** different sensor readings available. 
The samples have been divided into **two** classes where the class label is either 1 or -1. 
The class labels define to what particular class a particular sample belongs.

Your task is to **rank the sensors according to their importance/predictive power with respect to the class labels of the samples**.

Your solution should be a **Python**/R/Octave (for applicants with MATLAB experience) script that generates a ranking of the sensors from the provided CSV file.

The ranking should be in **decreasing order** where the first sensor is the most important one.

You get bonus points if you provide a solution that could in principle be scaled up to a much larger number of sensors.

---

## Pipeline

1. Load/Parse features

2. Load/Parse labels

3. Load/Parse feature names

4. Perform evaluation of feature importance with **Mean decrease impurity method** (Using `feature_importances_` measure from `RandomForestRegressor`, sklearn library)

5. Sort/Visualize the result

Useful article about selecting good feature is [HERE](http://blog.datadive.net/selecting-good-features-part-iii-random-forests/) 

## Result

![alt text][image1]

