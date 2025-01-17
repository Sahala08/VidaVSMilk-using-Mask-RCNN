
# VidaVSMilk-using-Mask-RCNN
The Repository is dependent on the algorithm of [Mask R-CNN](https://github.com/matterport/Mask_RCNN) and it can use to detect vida(one brand of draw out tissue) and milk(vita milk). 
* Notice: we use google colab to download, test, train, evaluate, visualize the model.  

# Download the weights 
Please download [it](https://drive.google.com/file/d/1HZ9i7IvWW7uSMMODVvPw7pHgKGjK5lKD/view?usp=sharing) and place on your repository root directory.

# Getting Started
* milkvsvida_demo.ipynb (in /samples) : Is the easiest way to start. It shows an example of using a model pre-trained on VidaVSMilk dataset (which is calibration by VIA) to segment objects in your own images.
* milkvsvida_0604.ipynb (in /samples/milkvsvida) : shows how to train Mask R-CNN on VidaVSMilk dataset. 
* detection_0614.ipynb (in /samples) : shows how to test on VidaVSMilk dataset and compute mAP.
* milkvsvida_demo.ipynb (in /samples) : A file to show the result of detectection and segmentation.
* model.py, utils.py, config.py: These files contain the main Mask RCNN implementation.

# Installation
Example is shown in samples/milkvsvida/maskrcnn_download.ipynb.

1. Clone this repository
2. Install dependencies
```bash
   pip3 install -r requirements.txt
   ```
   
3. Run setup from the repository root directory
```bash
   python3 setup.py install
   ```
4. Download pre-trained weights (
mask_rcnn_milkvsvida_0030.h5) from [google drive](https://drive.google.com/file/d/1HZ9i7IvWW7uSMMODVvPw7pHgKGjK5lKD/view?usp=sharing).

# Citation
```bash
   @misc{matterport_maskrcnn_2017,
     title={Mask R-CNN for object detection and instance segmentation on Keras and TensorFlow},
     author={Waleed Abdulla},
     year={2017},
     publisher={Github},
     journal={GitHub repository},
     howpublished={\url{https://github.com/matterport/Mask_RCNN}},
   }
   ```
