# Face Mask detection using Deep Learning (Transfer Learning)

As we know, there are couple of pre-trained Face Detection models available like Caffe Model or we can use Opencv Haar-cascasde classifiers for face detection. But how about if the model is able to detect mask as well if a person has wear mask or not during this pandemic.

Entire steps has been mentioned as follows :
## Dataset of images of people with Mask & Wihout Mask.
So, firstly we have taken a dataset of images for people with & without mask with around 2000 images. Thanks to Github for helping me getting the data.

## Training the model for Mask Detection
We have used the concept of Transfer Learning for Model creation. We have not created the model from scratch but we used the MobileNetV2 model as the base model & then trained it on our dataset so as to fine tune the existing model which saved us a lot of time. This process of using pretrained model & getting it fine-tuned with correct weights is called "Transfer Learning". 

## Face Detection
After training the mask detection model, we used caffe model to detect faces (we can use Haarcascade classifier as well) on real time images or video & then on face detected, we deployed the model we have trained to predict if person has wear mask or not on the face. So, we have followed two- step process here.
We have received an accuracy of around 99% using this process.

## License
[MIT](https://choosealicense.com/licenses/mit/)
