
## Kaggle Competition. Predict the yoga pose correctly!

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alex-agency/kaggle-yoga-pose-prediction/blob/main/yoga-pose-movenet.ipynb)

Human pose estimation is a well-known problem in computer vision to locate joint positions. The application of pose estimation for yoga is challenging as it involves a complex configuration of postures.

In this competition, pose estimation is formulated as a classification task, and it is necessary to classify different yoga asanas into distinct classes.

### Data Set
The dataset has pictures of different yoga poses and the class to which it belongs. There are a total of 6 classes based on the posture of the person performing the asana.

The dataset provided in the train.csv consists of the following features:
image_id: The unique ID for each image of yoga pose.
class_6: The class to which each yoga pose image belongs. (target variable)

The dataset consists of a train.csv file which contains the image_id and class_6 columns. The image_id is the unique id for each image of yoga pose and the class_6 classes of yoga poses to which that image belongs. The images for training and testing are present in the images folder. The aim of this competition is to predict the class_6 correctly for the test_images and submit the response as csv file submission.csv.

### Evaluation Metrics
The evaluation metric for this competition is Mean F1-Score. Submissions are evaluated on MeanFScore, which at Kaggle is actually a micro-averaged F1-score.

### Submission Format
For every image_id in the dataset, the submission file should contain two columns: image_id which is the unique id for each image from the testing images, and class_6 which is the class value to which the image belongs. The second column should be a space-delimited string value.

The file should contain a header and have the following format:

```
image_id,class_6
288795e9cfe594b29582c0ba5bb00d93.jpg,5
```