# line-detection-text-detection-object-detection
Idea which I want to impliment for the task
Line detection
For line detection I  used HoughLinesP opencv  library.i am getting good result in HoughLinesP as compare to HoughLines .
Text detection
For text detection the most accurate  was pytesseract library from python.although the text is not visible in last 3 or 4 images but I got good result  using pytesseract.
Object detection
Object detecton I used YOLO V5 model the data is very less for train but I did data agmentation and improve the accuracy littlebit .

HoughLinesP code
![image](https://user-images.githubusercontent.com/90651409/192339464-34d5fbf7-6ef9-4756-98d1-f95cb8f93ba2.png)
Output
![image](https://user-images.githubusercontent.com/90651409/192339604-5c3fbc9f-b88d-464c-91c5-214f58276613.png)
![image](https://user-images.githubusercontent.com/90651409/192339638-9ac064c4-812e-45e5-8380-58c224274488.png)


Pytesseract Code
![image](https://user-images.githubusercontent.com/90651409/192339917-5877282c-8fe6-42a2-b024-40965fcc53ff.png)
Output
![image](https://user-images.githubusercontent.com/90651409/192340025-238cbc6c-6614-464a-9e39-4299871c9de7.png)
![image](https://user-images.githubusercontent.com/90651409/192340159-50bd33a3-e095-4d61-b55f-c08c67becc4d.png)


labeling ,Data augmentation,YOLO train
 Train and validation
I split the data set into train and validation.8 image for train folder and 4 for validation
 Labeling
For labeling I used a website www.makesense.ai  and labeling all the train images and val images
 Data augmentation
Data is very less for YOLOV5 model so I did some data augmention method like rotated the image  clockwise and labeling all the rotated images
 Upload data and modified Yolo file
I uploaded the zip dataset into the collab and modified  the COCO128.yaml
 Training YOLO V5 model
Train the model I set the batch size is 60 and epoch is 1000.

