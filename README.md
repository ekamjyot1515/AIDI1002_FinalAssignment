# YOLOv5 Object Detection


---

## Introduction
This project demonstrates real-time object detection using the **YOLOv5** model. YOLOv5 (You Only Look Once) is a highly efficient model that can detect multiple objects in images and videos in real time. The aim of this project was to experiment with different configurations of YOLOv5 by adjusting parameters like model weights, input image size, and confidence thresholds, and to assess their impact on the model's performance.

---

## Project Structure
- **YOLOv5 Model**: Pre-trained on the COCO dataset, this model detects 80 different object classes.
- **Modified Parameters**:
  - Model weights (YOLOv5-small, YOLOv5-medium)
  - Image resolution
  - Confidence threshold for object detection
- **Evaluation Metrics**:
  - Precision
  - Recall
  - Frames Per Second (FPS)

---

## Methodology
1. **Dataset**: The model is pre-trained on the **COCO dataset**, which contains images of 80 common object classes.
2. **Model Variants**: 
   - YOLOv5-small for faster but less accurate detections.
   - YOLOv5-medium for a better balance between speed and accuracy.
3. **Parameter Tuning**: We experimented with different image sizes and confidence thresholds to optimize the model’s performance based on the needs of real-time detection.
4. **Evaluation**: Metrics such as precision, recall, and FPS were used to evaluate the performance of the model under various settings.

---

## Results
- **YOLOv5-small**: Provided faster detections but with slightly less accuracy, suitable for use in systems where speed is critical.
- **YOLOv5-medium**: Offered the best trade-off between speed and accuracy, making it ideal for scenarios that require both.
- **Image Size**: Reducing image size increased FPS but reduced accuracy, particularly for smaller objects.
- **Confidence Threshold**: A higher threshold reduced false positives but increased the chance of missing smaller objects. A lower threshold improved recall but resulted in more false detections.

---

## Performance Metrics
- **Accuracy**: YOLOv5-medium achieved the best balance between precision and recall.
- **FPS**: Achieved higher FPS rates with lower image resolutions, making it suitable for real-time applications.
- **Precision & Recall**: Adjusting the confidence threshold allowed for better control over false positives and missed detections.

---

## Future Work
1. **Feature Enhancements**: Explore additional features to improve accuracy.
2. **Additional Datasets**: Test the model on other large-scale datasets for robustness.
3. **Hardware Optimization**: Implementing YOLOv5 on hardware like GPUs and edge devices to enhance real-time performance.

---

## Repositories
- **Official YOLOv5 GitHub**: [YOLOv5](https://github.com/ultralytics/yolov5)
- **Project Repository**: [AIDI1002_FinalAssignment]((https://github.com/ekamjyot1515/AIDI1002_FinalAssignment))

---

## References
- **YOLOv5 Documentation**: [YOLOv5 GitHub](https://github.com/ultralytics/yolov5)
- **YOLOv4 Paper**: Bochkovskiy, A., Wang, C.-Y., & Liao, H.-Y. M. (2020). YOLOv4: Optimal Speed and Accuracy of Object Detection. arXiv [arXiv:2004.10934](https://doi.org/10.48550/arXiv.2004.10934)
