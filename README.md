# YOLO Object Detection Demo (Coin Classification)

This project demonstrates training and deployment of a YOLO object detection model using a custom dataset.  
The dataset used here contains images of coins (penny, dime, nickel, quarter), and the model was trained to detect and classify them.  
The same methodology can be extended to domain-specific tasks such as detecting **trees, waterbodies, or other aerial objects**.

---

##  Project Objective
To train a YOLO model on a custom dataset and evaluate its performance in detecting and classifying multiple object categories.

---

## 🛠 Methodology
1. **Dataset Preparation**  
   - Collected and labeled coin images into training and validation sets.  
   - Annotations prepared in YOLO format.  

2. **Model Training**  
   - Used YOLOv11 (small variant: `yolo11s.pt`).  
   - Trained for **60 epochs** at **640x640 resolution**.  
   - Training tracked metrics like mAP, precision, recall.  

3. **Evaluation**  
   - Model evaluated on validation dataset.  
   - Metrics visualized in `results.png`.  

4. **Inference**  
   - Tested on unseen images and video streams.  
   - Bounding boxes drawn with predicted labels and confidence scores.  

5. **Deployment**  
   - Best model weights saved as `best.pt`.  
   - Model successfully run locally using a Python script for real-time inference.  

---

## 📊 Results
- Model achieved promising accuracy in detecting and classifying coins.  
- Example performance metrics are saved in the `runs/detect/train/` folder.  
