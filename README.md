# Description
LVMI-YOLO is a low-light real-time object detection algorithm that employs LVP-Net for feature extraction, MIP-Net for low-light image processing, and DEL-Detect for simplified model architecture. By integrating NWD loss to optimize small object detection, it significantly enhances detection accuracy and efficiency.The model was tested on four low-light public datasets, validating its effectiveness.
# Download
The dataset and model have been released.

https://pan.baidu.com/s/1xt9fPDDzOKWBO2wAG567iw 提取码: 1234 
# Key Algorithm Description and Implementation
Enhancing Real-Time Object Detection in Low-Light and Complex Scenarios
  This model is based on YOLOv11, with improvements made in three areas: the backbone network, the neck network, and the detection head. The backbone network enhancements include the introduction of the LoG-Stem module, whose code is stored in YOLOV11V12/ultralytics-yolo11-main/ultralytics/nn/extra_modules/block.py. Detailed implementation of this module is available here. The C3K2 module has been modified into C3K2-VSS. The improved model code is stored in YOLOV11V12/ultralytics-yolo11-main/ultralytics/nn/extra_modules/mamba_vss.py, The detailed implementation of this module is available here. It introduces the PSConv convolution, with the module code stored in YOLOV11V12/ultralytics-yolo11-main/ultralytics/nn/extra_modules/block.py. The detailed implementation of this module is available here.
  Improvements to the neck network include: introducing a hierarchical kernel attention mechanism, whose code implementation is located at YOLOV11V12/ultralytics-yolo11-main/ultralytics/nn/extra_modules/MKDA.py. where the detailed implementation of the module can be found. The introduction of the illumination-guided attention (IGAB) module, whose implementation code is located at YOLOV11V12/ultralytics-yolo11-main/ultralytics/nn/extra_modules/attention.py, where the detailed implementation of this module can be found.
  The detailed code for the detector head improvements is located in `YOLOV11V12/ultralytics-yolo11-main/ultralytics/nn/extra_modules/head.py`, where you can find the full implementation of this code.
  For the detailed implementation and workflow of the algorithm, please refer to the code and paper provided above.
# For dependency packages and installation requirements, refer to the model's README file.
