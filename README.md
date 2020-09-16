# Second-Nurse-Care-Activity-Recognition-Challenge-2020 
URL : https://abc-research.github.io/nurse2020/
# Abstract
Sensor-based human activity recognition has become one of the challenging and emerging research areas. Several machine learning algorithm with appropriate feature extraction has been used to solve human activity recognition task. However, recent research mainly focused on various deep learning algorithms, our focus of this study is measuring the performance of traditional machine learning algorithms with the incorporation of frequency-domain features. Because deep learning methods require a high computational cost. In this paper, we used Naive Bayes, K-Nearest Neighbour, SVM, Random Forest and Multilayer Perceptron with necessary feature extraction for our experimentation. We achieved the best performance for K-Nearest Neighbour. Our experiment was a part of "The 2nd Nurse Care Activity Recognition Challenge Using Lab and Field Data" followed by the team MoonShot_BD. We concluded that with proper feature extraction, machine learning techniques may be useful to solve activity recognition with a low computational cost.
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
Google Colab, Numpy, Pandas, Tensorflow, Keras.
# Result 
Our team got first in the challenge.
