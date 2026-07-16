# Synthetic-Debris
# FBENet: A Highway Road Debris Detection Network

This repository provides the inference code and pre-trained model weights for the paper:  
**"FBENet: A Highway Road Debris Detection Network Based on Frequency-Aware Bidirectional Feature Fusion and Efficient Attention Enhancement"** (Submitted to *Sensors*).

## 📌 Quick Overview
- **Dataset**: Synthetic-Debris (brick, paper box, rock)
- **Model**: FBENet (improved from YOLO11n with FreqFusion-BiFPN and EMA)
- **Key Results**: 0.862 mAP@0.5, 0.811 F1-score on Synthetic-Debris

## 🗃️ Dataset Availability
- **Openly available part (8,000+ images)**: This portion of the Synthetic-Debris dataset is released in this repository under the dataset/ directory. It is provided under the CC BY-NC 4.0 license, pending final institutional approval. Should access via GitHub be interrupted or this repository be taken down for reasons beyond our control, the data will also be made available from the corresponding author upon reasonable request for research purposes.
- **Restricted part (~3,000 images)**: These images include corporate third-party assets that we are unable to redistribute. If needed, we can provide the source so that interested researchers may obtain them directly from the original providers.


## 🚀 Quick Start
```bash
# Clone this repository
git clone https://github.com/Chenyg0126/FBENet.git
cd FBENet

# Install dependencies
pip install -r requirements.txt

# Run inference (once you download the weights)
from ultralytics import YOLO
model = YOLO('weights/fbenet.pt')
results = model('path/to/image.jpg', imgsz=800)
results[0].show()
```

## 📁 Repository Structure
```
FBENet/
├── weights/          # Pre-trained model weights
├── inference.py      # Inference script
├── requirements.txt  # Python dependencies
└── README.md         # This file
```

## 🏷️ License
The code in this repository is released under the **MIT License**.  
## 🏷️Dataset (openly producible subset)
Planned release under CC BY-NC 4.0, subject to final institutional clearance.
## 🏷️Third-party assets
Not redistributable; source documentation will be provided separately.


## 📧 Contact
For questions or issues, please contact: [406013576@qq.com]
