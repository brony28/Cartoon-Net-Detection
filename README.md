# Cartoon-Net-Detection
Cartoon Detection using Faster R-CNN

Create a folder named Preparation. <br>
Keep the following things inside the Preparartion folder:<br>
1. a folder named **images** <br>
2. faster_rcnn_inception_v2_pets.config<br>
3. generate_tfrecord.py<br>
4. labelmap.pbtxt<br>
5. train.py<br>
<br>
<br>
The images folder will have 2 folders - <br> 
a. **test** <br>
b. **train** .
<br><br>
The train folder will have all the annotated training images and its corresponding xml file.
The test folder will have all the annotated testing images and its corresponding xml file.
The testing images should be less than training images. In this project, only 7 images were used for testing dataset.
<br><br>
labelmap.pbtxt will store the classes that is used in detection. In this project, 5 classes are used.
<br><br>
Next, in the generate_tfrecord.py file, update the function _class_text_to_int()_ with the class names used in the project. 
<br><br>
In faster_rcnn_inception_v2_pets.config file, update the number of classes _num_classes:_ with your classes count. And number of examples _num_examples:_ with the count of number of test images you included.
<br><br>
No need to edit the train.py
