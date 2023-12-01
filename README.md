# Sign-Language-Detection-mediapipe
This project was made with a target to classify the hand gestures in a sign language. It uses a google framework called mediapipe to detect and track the hand and body features.
<br>
<br>
The following are the images of the interactive dataset collection you can use to record videos of yourself doing the signs/actions.
<br>
Press 'x' to switch to next sign press 'z' switch to previous sign.
<br>
<br>
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/1a5277af-88c2-4ede-bc9a-bb70ad5abb51" width="40%" />
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/be092034-d42e-4227-a859-c7973fa0010c" width="40%" />
<br>
<br>
Once the sign is selected, press 'q' to start the capture process.(capture 30 videos one by one each of 20 frames)
<br>
The collected videos maybe of more than 20 frames, you can make them 20 frames in the preprocessing step.(already done in the preprocessing notebook)
<br>
Once all the Videos are collected for a sign , it will be marked as done against the sign name.
<br>
<br>
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/57808610-204a-4c75-9ab8-ef98c20a7f1d" width="40%" />
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/c00607f4-c35a-4e3a-a980-2b619c94c3a7" width="40%" />
<br>
<br>
The augmentation notebook helps you augment your original videos(scale,shift and rotate)(1 video ---> 15 Augmented videos)
<br>
<br>
The following is just a preview of the first frame of augmented video for different signs.
<br>
<br>
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/0b2fefdf-eef0-48ee-9cab-33336be7869f" width="80%" />
<br>
<br>
Preprocessing notebook extracts all the keypoints/landmarks from the augmented videos in the form of **[lefthand_landmarks,pose_landmarks,righthand_landmarks]** for each frame in each video.
<br>
<br>
So, the for each video, tensor will look like **(20,258)**.
<br>
<br>
Train the model with batches of these sequences of extracted keypoints.
<br>
<br>
**The following are the images of live sign language detection in action.**
<br>
<br>
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/082b36cb-0494-4c5f-8d4e-668ba4d7c9f6" width="40%" />
<img src="https://github.com/Viditnegi/Sign-Language-Detection-mediapipe/assets/106267998/3ee06111-5339-4f88-8ee9-faeb10ba2e64" width="40%" />
<br>
<br>


