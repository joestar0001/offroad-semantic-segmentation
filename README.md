# offroad-semantic-segmentation
Semantic segmentation model using a DINOv2 transformer backbone for off-road scene understanding. Includes trained weights, evaluation metrics, inference scripts, and performance analysis. Achieves 0.3185 mean IoU on validation set.
# Semantic Segmentation Model — Hackathon Submission

## 📌 Overview

This project presents a deep learning–based semantic segmentation model designed to segment off-road scene images into meaningful pixel-level categories. The model is trained using a transformer-based backbone and optimized for accurate region prediction and robust generalization.

---

## 🧠 Model Architecture

* **Backbone:** DINOv2 Vision Transformer
* **Framework:** PyTorch
* **Task:** Semantic Segmentation
* **Output:** Pixel-wise segmentation masks

---

## 📊 Performance Metrics

Validation performance achieved during training:

| Metric         | Score      |
| -------------- | ---------- |
| Mean IoU       | **0.3185** |
| Dice Score     | **0.4385** |
| Pixel Accuracy | **0.7025** |

These results demonstrate stable convergence and consistent validation improvement.

---

## 📁 Project Structure

```
FINAL_SUBMISSION/
│
├── segmentation_head.pth   → trained model weights
├── test_segmentation.py    → inference script
├── training_log.txt        → training history
├── config.txt              → model configuration
├── REPORT.txt              → evaluation summary
├── all_metrics_curves.png  → training graphs
```

---

## ▶️ How to Run Inference

```bash
python test_segmentation.py --model_path segmentation_head.pth --data_dir <images>
```

Predicted masks will be saved automatically.

---

## 📈 Training Behavior

Training curves show:

* steady loss decrease
* increasing IoU
* improving Dice score
* stable validation trend

This indicates correct optimization and good learning dynamics.

---

## ⚠️ Failure Case Analysis

Observed limitations:

* small object segmentation errors
* boundary imprecision
* texture similarity confusion

---

## 🚀 Possible Improvements

Future enhancements could include:

* higher input resolution
* stronger data augmentation
* deeper decoder head
* longer training schedule

---

## 🏁 Conclusion

The submitted model successfully performs semantic segmentation with stable training dynamics and competitive validation performance. The solution is reproducible, well-structured, and ready for evaluation.

---

## 👨‍💻 Author

Hackathon Participant Submission
