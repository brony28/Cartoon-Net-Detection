# Cartoon-Net-Detection
Cartoon Detection using Faster R-CNN

## Steps:

#### Setup:
Create a folder named Preparation. <br>
Keep the following things inside the Preparartion folder:
1. a folder named **images**
2. faster_rcnn_inception_v2_pets.config
3. generate_tfrecord.py
4. labelmap.pbtxt
5. train.py


The images folder will have 2 folders:
1.  __test__
2. __train__


The train folder will have all the annotated training images and its corresponding xml file.
The test folder will have all the annotated testing images and its corresponding xml file.
The testing images should be less than training images. In this project, only 7 images were used for testing dataset.
<br><br>
labelmap.pbtxt will store the classes that is used in detection. In this project, 5 classes are used.
<br><br>
Next, in the generate_tfrecord.py file, update the function `class_text_to_int()` with the class names used in the project. 
<br><br>
In faster_rcnn_inception_v2_pets.config file, update the number of classes `num_classes:` with your classes count. And number of examples `num_examples:` with the count of number of test images you included.
<br><br>
No need to edit the train.py
<br><br>
Now zip the Preparation Folder and upload the zipped file on the Google Drive.(Preferably inside a folder.)<br>
Upload the jupyter notebook files as well on the drive.<br>

#### Training the model
Open the notebook, __Part 1: Training Model using final_faster_rcnn.ipynb__ and run every cell.<br>

### Testing the model
Open the notebook, __ __ and run every cell.<br>

### TF to TFLite Conversion
Open the notebook, __ __ and run every cell.<br>
