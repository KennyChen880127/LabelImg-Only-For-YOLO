# LabelImg-Only-For-YOLO-Code
This project aims to modify and simplify the functionality of LabelImg, reducing the chance of errors caused by annotators who may not be familiar with the AI domain and may accidentally skip or misinterpret steps. The application exclusively supports the YOLO annotation format, with the added feature of automatic saving. It also automatically sets the annotation storage format and checks whether the input class matches the default value.

## LabelImg
[LabelImg](https://github.com/HumanSignal/labelImg) is an open-source graphical image annotation tool designed to annotate images for machine learning projects. It provides a user-friendly interface for drawing bounding boxes around objects in images, making it a valuable tool for creating annotated datasets. LabelImg supports various annotation formats, including the popular YOLO format, making it versatile for different machine learning tasks. The tool allows users to define and label classes, draw bounding boxes, and save annotations in a format compatible with training models. Additionally, LabelImg includes features such as automatic saving to streamline the annotation process and enhance workflow efficiency.


## Steps to run Code
### Create Virtual Environment
* First, make sure you have installed Python, and it is recommended to upgrade pip first.

		pip3 install --upgrade pip

* Install virtual environment.

  		pip3 install virtualenv

* Clone the repository and navigate to the project directory.

  		git clone https://github.com/KennyChen880127/LabelImg-Only-For-YOLO-Code.git

  		cd LabelImg-Only-For-YOLO-Code
  
* Create a virtualenv.

  		virtualenv env
  
  		cd env\Scripts

  		activate

* Install the required packages: PyQt5 and lxml.

		pip3 install pyqt5 lxml
  
* Use pyrcc5 to convert the file configured in resources.qrc to resources.
  
		pyrcc5 -o libs/resources.py resources.qrc

* Set up the predefined classes by configuring the data/predefiend_classes.txt file with the following format:

		person
  		dog
		cat
  
* Execute LabelImg.py.

		python labelImg.py

* If you need to package LabelImg.py into an executable (.exe) file, use the following command:

		pip3 install pyinstaller
		pyinstaller --hidden-import=pyqt5 --hidden-import=lxml -F -n "labelImg" -c labelImg.py -p ./libs -p ./
