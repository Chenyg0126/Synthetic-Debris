# Synthetic-Debris
# FBENet: A Highway Road Debris Detection Network

This repository provides the inference code and pre-trained model weights for the paper:  
**"FBENet: A Highway Road Debris Detection Network Based on Frequency-Aware Bidirectional Feature Fusion and Efficient Attention Enhancement"** (Submitted to *Sensors*).

## 📌 Quick Overview
- **Dataset**: Synthetic-Debris (brick, paper box, rock)
- **Model**: FBENet (improved from YOLO11n with FreqFusion-BiFPN and EMA)
- **Key Results**: 0.862 mAP@0.5, 0.811 F1-score on Synthetic-Debris

## 🗃️ Dataset Availability
- **Openly available part (8,000+ images)**: The majority of our Synthetic-Debris dataset will be released on Zenodo under the **CC BY-NC 4.0** license. A persistent DOI will be provided upon publication.
- **Restricted part (~3,000 images)**: These images were sourced from third-party data and cannot be redistributed. Documentation on data sources is available upon request.

## 🚀 Quick Start
```bash
# Clone this repository
git clone https://github.com/user1236/FBENet.git
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
The openly available part of the Synthetic-Debris dataset is released under the **CC BY-NC 4.0** license.


## 📧 Contact
For questions or issues, please contact: [406013576@163.com]
