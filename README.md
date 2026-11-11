# NEUCAR Horizon Vision Assessment 2026

**地平线视觉组考核 · Horizon Vision Group Assessment**

基于智能车竞赛 ROS 2 Bag 数据的视觉算法实践考核。  
A practical computer vision assessment using ROS 2 Bag data from an autonomous car competition.

## 考核内容 / Tasks

**01 · 锥桶检测与 BEV 映射 / Cone Detection & BEV Mapping**  
使用 YOLO 检测锥桶，将检测框底边中点映射至 BEV，并生成矩形障碍物区域。  
Detect cones with YOLO, project bounding-box bottom centers into BEV, and represent obstacles with rectangles.

**02 · 行驶参考轨迹提取 / Reference Trajectory Extraction**  
提取通道中心线，并处理锥桶避障与弯道场景。  
Extract lane centerlines and generate reference trajectories for obstacle avoidance and turns.

## 资料 / Resources

- [考核说明 / Assessment PDF](./地平线视觉组考核.pdf)
- [数据集下载 / Dataset download](./数据集下载链接.txt)
- [棋盘格 / Checkerboard PDF](./calib.io_CHECKERBOARD_200x200_11x11_15.pdf)
- 参考图像 / Reference images: [reference.jpg](./reference.jpg) · [reference2.jpg](./reference2.jpg)

## 验收 / Evaluation

需完成**现场实时摄像头测试**与**独立测试集测试**。BEV 变换允许预先标定，正式运行时须自动加载参数，无需重新选点。  
Both **live-camera** and **held-out test-set** evaluations are required. BEV calibration may be performed in advance; the program must load saved parameters without manual point selection at startup.

具体要求以考核 PDF 为准。 / See the assessment PDF for full requirements.
