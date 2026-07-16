# Synthetic-Debris
Highway road debris detection dataset (brick, paper box, rock)
FBENet: A Highway Road Debris Detection Network

、# FBENet: A Highway Road Debris Detection Network

This repository provides the inference code and pre-trained model weights for the paper:  
**"FBENet: A Highway Road Debris Detection Network Based on Frequency-Aware Bidirectional Feature Fusion and Efficient Attention Enhancement"** (Submitted to *Sensors*).

## 📌 Quick Overview
- **Dataset**: Synthetic-Debris (brick, paper box, rock)
- **Model**: FBENet (improved from YOLO11n with FreqFusion-BiFPN and EMA)
- **Key Results**: 0.862 mAP@0.5, 0.811 F1-score on Synthetic-Debris

## 🚀 Quick Start
```bash
# Clone this repository
git clone https://github.com/your-username/FBENet.git
cd FBENet

# Install dependencies
pip install -r requirements.txt

# Run inference (once you download the weights)
from ultralytics import YOLO
model = YOLO('weights/fbenet.pt')
results = model('path/to/image.jpg', imgsz=800)
results[0].show()
