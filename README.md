# Activity-Recognition-using-Accelerometer-Data
This project is mostly our experimentation on Activity Recogtion Problem based of Accelerometer Data using different Supervised Learning Algorithms.
# Datasets
The dataset was collected from the Second Nurse Care Activity
Recognition Challenge “From lab to field” under the HASCA Workshop in Ubicomp 2020. The data was collected using accelerometer
sensor in mobile phone.
# Preprocessing
What we had is positional x, y and z values against each timestamp
in the whole dataset directly collected from the accelerometer. The
raw data that we get from accelerometer is scattered and noisy. So
at first we processed the raw data through filters and normalized it.
We merged the label data with the sensor datafile and dropped irrelevant extra points.
# Feature Extraction 
After dividing the data into convenient window size we extracted
summarizing features from them. We calculated general values like
mean, median, mode for all the frames. To find the intermediate
relation between each data within a frame we calculated variance.
We also took standard deviation as a feature to see how much spread
out the data can be in any individual activity frame.
# Training and Testing 
After preprocessing, framing and necessary feature extraction, we
split them into training and testing dataset keeping the 80-20 ratio
and shuffling them randomly. The training dataset is used to train
the recognition model and testing dataset is used to verify the
accuracy of the model. 
# Recognition 
We used KNN, Naive Bayes, SVM, Random Forest and Softmax Regression with Deep Neural Networks. Among them, Softmax Regression was the fastest and KNN was the most accurated.
# Framework and IDE 
Google Colab, Numpy, Pandas, Tensorflow, Keras,
