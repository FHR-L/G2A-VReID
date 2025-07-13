## G2A-VReID & G2A-VReID.v2

### Introduction
G2A-VReID is a large-scale video-based pedestrain Re-Identification datasets, constructed by National Engineering Laboratory for Integrated 
Aero-Space-Ground-Ocean (ASGO) Big Data Application Technology. G2A-VReID consists of 2,788 person IDs and 185,907 images, 
corresponding to 5,576 tracklets. The number of identities is significantly higher than most of existing datasets. To
best of our knowledge, G2A-VReID is the first dataset for video ReID under Ground-to-Aerial scenarios. 
G2A-VReID dataset has the following characteristics: 
1) Drastic view changes; 
2) Large number of annotated identities;
3) Rich outdoor scenarios;
4) Huge difference in resolution.

G2A-VReID.v2 is an extended large-scale video-based pedestrian Re-Identification dataset. Compared to its predecessor, G2A-VReID.v2 significantly expands the dataset scale and complexity, containing 5,605 person IDs, 2.54 million images, and 11,282 tracklets, making it one of the largest publicly available video ReID datasets to date.
The dataset possesses the following key characteristics:
1) Extreme cross-viewpoint variations, including top-down and oblique angles from UAVs and conventional ground-level views;
2) Large-scale identity and video tracklet annotations, more than doubling the size of the original G2A-VReID;
3) Rich environmental diversity, covering 13 outdoor scenes such as construction sites, plazas, flyovers, and grasslands;
4) Wide resolution disparity, especially under high-altitude UAV views;
5) Multi-season and day-night coverage, capturing diverse lighting, weather, and appearance conditions across time.

### Privacy Protection
We try our best to protect the privacy of pedestrians from the following aspects:
1) we make our best efforts to inform pesdestrains about data collection, 
cordons are used to mark data collection areas and notifications (including ) are 
post near the sites in collection process. 
![img.png](./images/notification.png)
2) To further minimize privacy risks, 
we use mosaic mask the clear face information. Sepecially, we construct a 
face detection model (FDM) based on YOLOv5, which are trained on 
both widerface-m and darkface-m datasets. Then, the FDM is empoly to mark out 
clear face of pedestrains, and the masking them by mosaic (RGB:[96, 96, 96]). Meanwhile, 
10 experienced annotators are employed to check for missing detection images 
and mask them by manual.
![img_1.png](./images/img_1.png)
3) Finally, the dataset will be licensed for non-profit academic 
research only, any researcher who downloads the G2A-VReID dataset must agree to observe the restrictions. 
![img.png](images/agreement.png)

### Request For G2A-VReID and G2A-VReID.v2
G2A-VReID is available at [Link](https://drive.google.com/file/d/1vPS-Xc1gBNc8Q40QZ0FaUWeYRkKsndeL/view). G2A-VReID.v2 is available at [Link](https://drive.google.com/file/d/15pkbcPP5dm4G7lZGpPYG8tSvF8zQ5USQ/view?usp=sharing). If the link becomes invalid, please feel free to contact luowenlong@mail.nwpu.edu.cn.
### Citaion
```
@inproceedings{zhang2024cross,
  title={Cross-platform video person reid: A new benchmark dataset and adaptation approach},
  author={Zhang, Shizhou and Luo, Wenlong and Cheng, De and Yang, Qingchun and Ran, Lingyan and Xing, Yinghui and Zhang, Yanning},
  booktitle={European Conference on Computer Vision},
  pages={270--287},
  year={2024},
  organization={Springer}
}
```
```
