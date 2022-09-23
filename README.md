# Seatbelt-Phone-Violation-Detector
Detecting Seatbelt and Phone violations using AI..How it works, let's see>>

## We have done this project using two models:

### The first model's task is to detect where is the windshield in the image, as an example see this image:
![savedImage](https://user-images.githubusercontent.com/80279479/186296710-7ba621c1-697d-4e6a-8ae5-0d602fa3a060.jpg)

The first model was built using object detection API with pre-trained model named `my_ssd_resnet50_v1_fpn`.
After detecting the windshield, we take the coordinates of the windshield and cut the image and fed it into the second model.
source code: https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/training.html

### The second model's task is to detect the type of violation in the image:
![windsheld__0a7f649d-c89b-11ec-92f9-2cf05d25561e](https://user-images.githubusercontent.com/80279479/186297389-25523ce8-6c8f-4a79-acd4-ff0807311045.JPG)
The second model was built using image classification pre-trained model named `VGG19`.
You will see the training source code and details in the file `Classification.ipynp`.


You can try the project through this website:
http://157.175.176.119
