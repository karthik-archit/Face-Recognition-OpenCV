# Face-Recognition-OpenCV

Overview:

Facial recognition involves 2 steps , detecting the face in an image then classifying the image. OpenCV’s facial detection model is used to detect faces and then pre-trained facenet model is used to extract face embeddings and a simple feed forward network is used to classify the images.

Dataset Used:

Custom dataset of football players from the internet.

Libraries Used :

Keras , Tensorflow, Open CV, Numpy , sklearn

Project Flow:

1) Training and Evaluation:

Read image -> Resize image and subtract mean values of each channel from the image -> Detecting the face using open cv face detector -> Only use detections which have a confidence more than 60 percent -> Extract the height and width of detected faces -> Crop the face from the image using the extracted height and width -> Pass the extracted face to facenet to extract face embeddings -> Train a simple feed-forward network using the extracted embeddings to classify the faces.

2) Inference :

Repeat the same steps used in the training process to extract face embeddings -> Predict the face -> Apply bounding boxes of detected faces along with their predicted class as label and its corresponding probability.

This project helped in understanding the intuition behind facenet , triple loss in training the facenet model, face Embeddings . It also helped me in using OpenCV for image processing , applying bounding boxes and also its dnn module to use neural network models.
