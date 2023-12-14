# LabelImg-Only-For-YOLO
This project aims to modify and simplify the functionality of LabelImg, reducing the chance of errors caused by annotators who may not be familiar with the AI domain and may accidentally skip or misinterpret steps. The application exclusively supports the YOLO annotation format, with the added feature of automatic saving. It also automatically sets the annotation storage format and checks whether the input class matches the default value.

![Example_1](https://github.com/KennyChen880127/LabelImg-Only-For-YOLO/blob/master/example_1.jpg)

## LabelImg
[LabelImg](https://github.com/HumanSignal/labelImg) is an open-source graphical image annotation tool designed to annotate images for machine learning projects. It provides a user-friendly interface for drawing bounding boxes around objects in images, making it a valuable tool for creating annotated datasets. LabelImg supports various annotation formats, including the popular YOLO format, making it versatile for different machine learning tasks. The tool allows users to define and label classes, draw bounding boxes, and save annotations in a format compatible with training models. Additionally, LabelImg includes features such as automatic saving to streamline the annotation process and enhance workflow efficiency.


## Steps to run EXE
1. Click on <>Code, and select "Download ZIP" from the dropdown menu.
2. After extracting, go into the LabelImg-Only-For-YOLO-master folder and run labelImg.exe to start annotation.
3. Alternatively, you can modify the default class names in data/predefined_classes.txt. The sample format is as follows:

		person
  		dog
		cat
