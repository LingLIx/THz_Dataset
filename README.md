# Active Terahertz Imaging Dataset for Concealed Object Detection
-[Project Page & Dataset](https://linglix.github.io/THz_Dataset/)
****
## Introduction
Concealed object detection in Terahertz imaging is an urgent need for public security and counter-terrorism. In this paper, we provide a public dataset for evaluating multi-object detection algorithms in active Terahertz imaging resolution 5 mm by 5 mm.  To the best of our knowledge, this is the first public Terahertz imaging dataset prepared to evaluate object detection algorithms. Object detection on this dataset is much more difficult than on those standard public object detection datasets due to its inferior imaging quality. Facing the problem of imbalanced samples in object detection and hard training samples, we evaluate four popular detectors: YOLOv3, YOLOv4, FRCN-OHEM, and RetinaNet on this dataset. Experimental results indicate that the RetinaNet achieves the highest mAP. In addition, we demonstrate that hiding objects in different parts of the human body affect detection accuracy. The dataset will be available online.

## Dataset
Sample display for each category. The bottom row shows a zoomed-in view of the object.
![image1](/Image/classes.png)


Sample display for diversification.
![image2](/Image/diversification.png)

### Dataset structure:
```
/THZ_dataset_det_VOC
    /Annotations
        /D_N_F1_CK_F_LA_WB_F_S_back_0907140917.xml
        /D_N_F1_CK_F_LA_WB_F_S_front_0907140917.xml
        /D_N_F1_CL_V_LA_LW_V_RA_back_0907141138.xml
        /...
        /T_P_M6_MD_F_LL_CK_F_C_WB_F_RT_front_0906154134.xml
    /JPEGImages
        /D_N_F1_CK_F_LA_WB_F_S_back_0907140917.jpg
        /D_N_F1_CK_F_LA_WB_F_S_front_0907140917.jpg
        /D_N_F1_CL_V_LA_LW_V_RA_back_0907141138.jpg
        /...
        /T_P_M6_MD_F_LL_CK_F_C_WB_F_RT_front_0906154134.jpg
```

## Download links:
- [Google drive](https://drive.google.com/drive/folders/1A6LiyWAvRmKIJN5yXQZ3HxZVwNEFz8uV?usp=sharing)
- [Baidu drive](https://pan.baidu.com/s/1MRPyeMtzCQRO5ydgX0rSHA)(Extraction code: x3od)
- [NUAA drive](https://pan.nuaa.edu.cn/share/5cb047f309049ba7f68ab9e1e0)

---


**If you find this dataset useful in your research, please consider citing:**

```

```
