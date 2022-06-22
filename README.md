Model: Yolov4-tiny
Training Code: YOLOv4_tiny_Darknet_Parking.ipynb
For training use your own roboflow api key.

Dataset : UFPArk raw data
https://nextcloud.lasseufpa.org/s/qxWsqNjLSgqqdHM

Processed Dataset:
https://app.roboflow.com/tiny-yolo-v4-y89yh/cnn-hack/1

Implementation:
Yolo-in-cv2-video.ipynb
1 cell for Photos Implementation
2 cell for Video Implementaion

Model Details:
calculation mAP (mean average precision)=96
detections_count = 3434, unique_truth_count = 2758  
class_id = 0, name = empty, ap = 81.96%   	 (TP = 936, FP = 159) 
class_id = 1, name = parked, ap = 98.90%   	 (TP = 1560, FP = 84) 
class_id = 2, name = unauthorized, ap = 88.54%   	 (TP = 21, FP = 2) 

for conf_thresh = 0.25, precision = 0.91, recall = 0.91, F1-score = 0.91 
for conf_thresh = 0.25, TP = 2517, FP = 245, FN = 241, average IoU = 78.84 % 

IoU threshold = 50 %, used Area-Under-Curve for each unique Recall 
mean average precision (mAP@0.50) = 0.898009, or 89.80 % 

Impementaion Details:
FPS 24-30 While displaying output
FPS 45-50 While processing only
