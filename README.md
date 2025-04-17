# multi-modal-fetal-abnormality-detection-ai

**AI for Early Detection of Fetal Abnormalities**


AI system for early detection of fetal abnormalities using a multi-modal approach that combines ultrasound images and non-invasive ECG signals to identify brain malformations (CSP, LV) and cardiac arrhythmias through real-time, automated predictions.
Traditional fetal anomaly screening methods could be reliant on subjective interpretation of ultrasound scans and fetal heart rhythm monitoring, with limitations due to subjectivity, operator variability, and detection at late gestational ages. Our approach differs by combining the application of deep learning algorithms in order to enable automation and enhanced diagnostic accuracy with real-time and non-invasive assessment of abnormalities in brain structure as well as in cardiac rhythm abnormalities.
---

### 📁 Project Directory Structure
```text
📂 ECG/
│   ├── ECG_Model.ipynb                 # ECG model notebook
│   ├── ecg_cnn_lstm_final.pth          # Trained ECG model
│   └── Dataset2_NonInvasive/
│       ├── set-a/
│       │   └── set-a/                  # Raw ECG data (.hea, .dat, .fqrs, .fqrs.txt, .csv)
│       └── set-b/
│           └── set-b/                  # Raw ECG data (.hea, .dat, .csv)

📂 Ultrasound/
│   ├── Ultrasound_Model.ipynb          # Ultrasound model notebook
│   ├── ultrasound_resnet_model.pth     # Trained ResNet18 model
│   ├── test/                           # Test set for evaluation
│   │   ├── *.png                       # Test ultrasound images
│   │   └── _classes.csv                # Labels for test images
│   ├── train/                          # Training set
│   │   ├── *.png                       # Train ultrasound images
│   │   └── _classes.csv                # Labels for training images
│   ├── valid/                          # Validation set
│   │   ├── *.png                       # Validation ultrasound images
│   │   └── _classes.csv                # Labels for validation images
│   └── Dataset2/                       # Unlabeled fetal head images (generalization testing)

📄 Fusion_MODEL.ipynb                   # Fusion model notebook (ECG + Ultrasound)
📄 fusion_model.pth                     # Trained fusion model weights

📂 reports/                             # Grad-CAM visualizations and final prediction results
```
