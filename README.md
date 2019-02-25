# Cognitive Computing: Ship Image Recognition 
Hi all, this is a Data Science Project ! - Image Recognitions with CNN Deep Learning methodology.


### Project Objective

* The purpose of this project is to apply Deep Learning methodology for Image Recognitions in order to detect the real ships through satellites all over the ocean.


### Methods Used

* Inferential Statistics
* Data Cleansing
* Data Wrangling
* Deep Learning
* Predictive Modeling


### Algorithm Used

- Deeping Learning:

  - Convolutional Neural Network (CNN)
  
  
### Technologies and Packages Used

* Python, Jupyter Notebook
* Numpy, Pandas, Glob
* Tensorflow, Keras, Cv2


### Project Description

* Motivation:

  - There are tons of ships navigating all over the ocean every day, but only few can be detected by satellites or other means quickly and accurately. Certain routes may be of interest for regulating environmental disruption, monitoring ships at risk of piracy, and avoiding overcrowding.
  
  
* Data and Scope:

  - I used segments of satellite imagery submitted to the public by Airbus for use in a Kaggle classification competition. This dataset contains a database of more than 200,000 small images of tankers, commercial ships, or fishing ships. Therefore, I extract some sample data here and present the predictive results for demonstration.
  
  
* Convolutional Neural Network (CNN):

  - Convolutional layers apply a convolution operation to the input, passing the result to the next layer. The convolution emulates the response of an individual neuron to visual stimuli. Each neuron processes data only for its receptive field.
  
  
* Methodology Approach:

  - Data Cleansing:
    1. Convert all missing values into 0 and the rest into 1, so there are only **[0,1]** values insides.
    2. Rename columns into **Image** and **Existing**.
    3. Calculated the ratio of finding ships which is around 35% in this dataset.
   
  - Modeling Approach:
    1. Split the dataset into 80% training data and 20% testing data.
    2. Transfer all image files into tensorflow format for training with **Keras**.
    3. Build convolutional layers and train the data with batch_size = 20 and epochs = 20.
    4. Save the highest accuracy training model during processing.
    5. Test the model with new input data.

  
### Conclusion:

  - The accuracy of new testing model is around **65%** which is good. However, there are still some error images found from the outputs, the possible reason is **because sample data is not large enough** to get a better performance. In other words, the accuracy of this model will get higher if all the data are used for training. In general, this model can be applied to satellite images from any area of interest for ship detection and quantification with excellent performances.
  
  


