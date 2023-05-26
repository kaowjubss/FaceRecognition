# FaceRecognition
 Face Recognition for 5 people which are members in my group
 
## Data Acquisition
 Our data source is images of members in my group. There are 460 images for 5 classes.

## Data Preparation (Roboflow)
### upload all data to Roboflow
 upload all 460 images to roboflow.
<img
  src="/Readme_md/upload2roboflow.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
### Label and anotate the data
Label face and select class(name)
<img
  src="/Readme_md/anotation.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
### Augmentation
 select the augmentation type and set the value. We use rotate, shear, brithness, blur ,and noise for augmentation step and we get 2754 data for 5 classes
<img
  src="/Readme_md/augmentation.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
## Model Training and Deploy
follow the steps from yoloV5 in Github https://github.com/ultralytics/yolov5
1. clone from https://github.com/ultralytics/yolov5
2. create file.yalm 
   - set dataset folder
   - set number of class
   - set list of class name by order from roboflow
     <img
  src="/Readme_md/yaml.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
     <img
  src="/Readme_md/order.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
3. install wandb and login for result graph
   <img
  src="/Readme_md/wandb.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
5. train model 
   - pixel(640x640) and epoch 100 times. The data will get from coco.yaml and yolov5s.pt that we set from before.
     <img
  src="/Readme_md/train.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
5. result<br/>
   <img
  src="/Readme_md/result1.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
  <img
  src="/Readme_md/result2.png"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">
7. predict<br/>
   <img
  src="/Readme_md/detect.jpg"
  alt="Alt text"
  title="Optional title"
  style="display: inline-block; margin: 0 auto; max-width: 300px">

### Video link
https://youtu.be/meB0ZNBhG4k <br/>
https://vt.tiktok.com/ZSLRGTcaT/?t=1

  
  

