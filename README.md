# Realtime Indian Sign Language Detection 

Hand gestures are one of the methods used in sign language for communicating non-verbally. It is usually used by individuals with speech or hearing problems, in order to communicate.

We developed this project for Rotaract Club of Bombay Airport under their initiative "Tech for a Cause". This projects aim to be a stepping stone to help Mute and Deaf people communicate remotely using video conferencing tools. An automated system that recognizes these hand gestures, provides an innovative and user friendly way of communication by keeping in mind the similarities of human hand shape with four fingers and one thumb. 

Getting Started 

Pre-requisites 
Before running this project, make sure you have following dependencies -
1. Python 3.6 
2. pip 
3. Open CV 
4. Visual Studio Code 
5. Object Detection API 
6. Protobuf 
7. Cuda and Cudnn (if GPU is there in the system - optional) 

Now, use Installation Master Script, which will help install all the packages which arent already in your environment. 

Running
To run the project, perform following steps -

1. Run "Image Collection (WebCam).ipynb" - this ipynb will Collect Images directly from your webcam and save it in your folder named "CollectedImages" 
2. Run "Automate Labelling.ipynb" - this ipynb detects your hands using MediaPipe and retrieves rectangular coordinates of hand location.This ipynb generates XML files with the coordinates saved for each image. Set the path of all folders the same as where collected images are stored. 
3. Manually Separate test and train data. The folder location is the same as CollectedImages. Just copy and paste jpg and xml files into 80-20 ratio for train and test respectively. 
4. Run "New Model Training, Evaluation and Detection.ipynb" - make your own model by setting a new label map and then creating the tensorflow records. Eventually generating a final model, loss and evaluation matrices. After this image detection as well as Real-time (Webcam) detection is possible by running the last cells in the notebook. 

<Blog se copy paste>

Results 
![image](https://user-images.githubusercontent.com/84955516/120929931-b1b49600-c708-11eb-8a11-e1b5ae784b81.png)
![image](https://user-images.githubusercontent.com/84955516/120930049-44553500-c709-11eb-8dca-3e0487fca853.png)
![image](https://user-images.githubusercontent.com/84955516/120930057-4b7c4300-c709-11eb-8275-408df6d27a8d.png)




For more detailed explanation you can check out our blog here - 
1. Blog 1 
2. Blog 2 
