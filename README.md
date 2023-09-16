
## Yoga Pose Estimation - Kaggle Competition 
### Predict the yoga pose correctly!

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/alex-agency/kaggle-yoga-pose-prediction/blob/main/yoga-pose-movenet.ipynb) [![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://kaggle.com/kernels/welcome?src=https://github.com/alex-agency/kaggle-yoga-pose-prediction/blob/main/yoga-pose-movenet.ipynb)

### Description
Yoga, a practice known for its physical and mental benefits, gained widespread popularity, particularly during the past two years amid the global pandemic. With more people practicing yoga at home, the importance of correct posture during yoga sessions became paramount. This Kaggle competition tackled the challenge of human pose estimation in yoga, aiming to accurately classify various yoga asanas (poses) from images.

Human pose estimation is a well-known problem in computer vision to locate joint positions. The application of pose estimation for yoga is challenging as it involves a complex configuration of postures.

The competition framed the pose estimation as a classification task, with the goal of achieving high Mean F1 scores. The dataset consisted of images of different yoga poses, each labeled with its corresponding class based on the practitioner's posture. The complexity of yoga poses, including horizontal body postures and overlapping limbs, made this task particularly challenging.

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
