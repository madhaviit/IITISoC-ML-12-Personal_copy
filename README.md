The problem statement of our model was to give song recommendations by identifying facial expressions.
Basically, we had to build a computer vision model which will scan the face (live video feed) and based on the emotion of the person the machine will provide an appropriate song.

We have used a custom-trained CNN (Convolutional Neural Network) to detect emotion from Webcam input. The maximum accuracy achieved is 65.74%. 

Other models we used are:
ResNet50
MobileNet
VGG-19
RMN (Residual Masking Network)
However accuracy achieved was sub-par compared to the custom CNN except for one i.e. RMN. And RMN has much better accuracy, but sufffers from file- size restriction while we tried to host it globally. As a result we  had to host our custom CNN network globally instead using  streamlit. To access the webpage follow the URL mentioned below:

https://a5hu705h-streamlit-song-recommend--haar-recommend-songs-0smud8.streamlitapp.com/

The flask web application we wished to deploy on heroku still can be hosted locally. In order to do so, we require virtual environment installed with requiredd libraries viz., opencv-pyhton, flask, tensorflow, numpy. 
Once we are ready with our virual environment, we just need to run app.py

Alternatively, if you wish to access RMN implementation (with around 76% accuracy) in flask by hosting it locally, find it in the following repository.
https://github.com/cse210001015/Song-Recommender-System-RMN
Lastly, if you wish to host streamlit implementation of this model, use following repo:
https://github.com/cse210001015/song_recommender_RMN/blob/master/Recommend_Songs.py

