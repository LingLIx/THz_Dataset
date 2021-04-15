# An Active Terahertz Imaging Dataset for Concealed Multi-object Detection and Evaluation-[Project Page & Dataset](https://liling0.github.io/THz_ImageDataset/)

****
Concealed objects detection in Terahertz imaging is an urgent need for public security and counter-terrorism. So far, there is no public Terahertz imaging dataset for evaluation of objects detection algorithms. This paper provides a public dataset for evaluating multi-object detection algorithms in active Terahertz imaging worked at 140 GHz, with the imaging resolution 5 mm by 5 mm. Due to poor imaging quality, object detection on this dataset is much more difficult than on those commonly used public object detection datasets in computer vision field. Several state-of-the-art computer vision based detectors, including YOLOv3, YOLOv4, FRCN-OHEM and RetinaNet, are evaluated on this dataset. In addition, we enhance RetinaNet through embedding low-level features for detecting small objects. Aiming at solving the problem of unbalanced and hard training samples, Focal Loss and Online Hard Example Mining technology are discussed and employed. Experimental results show that the enhanced RetinaNet achieves the best mAP with fast detection speed which can meet the requirement of real-time security inspection. Experiment also indicates that hiding objects in different parts of the human body affect the detection accuracy.

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
