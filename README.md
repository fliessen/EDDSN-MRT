# EDDSN-MRT: Multiple Rodent Tracking Based on Ear Detection and Dual Siamese Network for Rodent Social Behavior Analysis
The source code for ***EDDSN-MRT: Multiple Rodent Tracking Based on Ear Detection and Dual Siamese Network for Rodent Social Behavior Analysis***.

Thanks for your interest in our work.



## Rquirements of EDDN
Cython    
matplotlib>=3.2.2   
numpy>=1.18.5   
opencv-python>=4.1.2   
Pillow   
PyYAML>=5.3    
scipy>=1.4.1    
tensorboard>=2.2    
torch>=1.6.0    
torchvision>=0.7.0    
tqdm>=4.41.0    


## Data preparation

  We do not provide the trainning data itself. You must label the object detection trainning data by yourself. Specifically, using software such as ***Labelme*** is an ideal approach.
  
## Run EDDN

1. Clone the repo.

       git clone https://github.com/fliessen/EDDSN-MRT/     
       cd EDDSN-MRT/  

2. Train a network.

       python train.py --weights weights/yolov5s.pt  --cfg models/EDDN_small.yaml  --data data/mydata.yaml --epoch 50 --batch-size 4   --device 0
       
3. Detect target.

       python detect.py --weights xxxxxxxx/best.pt --img 640 --source xxxxxxxx.png



       
