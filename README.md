# Problem - Face Detection with Deep learning's Single Shot Detection method

# Application - security, biometrics, photography, emotional intelligence, entertainment.
  # First step of Face recognition or Face verification is Face detection.

Solution :-

  > Network/Layer - Res10

  > Framework - Caffe

  > Library - cv2, numpy, matplotlib.pyplot 

  > Pipeline (Inderfence/testing) :-

      : Read the image.

      : Load the network's model file (stored trained weights). 
      
      : Load the network's config file (stored network's configuration / architexture detail).

      : Read the network's files using Caffe framework.

      : Convert the image into blob format- helps the network to understand the image through blob format. 
        Note- the parameters of blob function to convert image into blob is as per the newtwork's configuration text file.
      
      : Set the blob image ready and pass the blob forward to the to the loaded model for the face detection on the given input image.

      : The result of detection is list of list cardinally with confidence score, (x,y) coordinate, width, height.

      : Set the detection threshold value- detects how well the face is detected in the detected bounding box.

      : For each detections, extract the confidence score, check whether it satisfies with the detection threshold value. 
      
        - If yes, extract the bounding box dimensions and draw the bounding box with confidence score as a label.

        - Else no, then will pass to the next detection.
      
  > As the Face detecton model is designed with a motivation of SSD theory, the result from the input image will display the image with all valid face detection. 
