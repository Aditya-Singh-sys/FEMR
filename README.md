# FEMR
Facial Expression Music Recommender: An app that recommends music based on user's facial expression.

The project works as follows:
  - On pressing the "Scan" button, the program starts taking in the webcam feed.
  - For each frame of the feed, the program extracts faces using the haarcascade library.
  - Each face is converted to a 48x48 grayscale image which is passed to the trained CNN. 
  - The weighted mean of predictions from the CNN is calculated, the weights being the frame number
  - 10 songs are randomly selected from one of 7 collections(based on the average prediction)
  
