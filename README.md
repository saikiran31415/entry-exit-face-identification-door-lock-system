# Entry Exit Face Identification Door Lock System

## An AI-Powered Smart Security Solution

This project implements an intelligent entry-exit door lock system using face recognition and object detection technologies. The system combines machine learning models to provide secure, contactless access control for buildings and secure areas.

---

## Team Details

**Team Name**: Game Changers

| Team Member | Roll Number |
|-------------|-------------|
| Parvigari Sai Kiran Chary | 244101031 |
| Saireddy Shreyas | 244101046 |
| Vishnu Vardhan G | 244101066 |
| Rohan Jainarayan Dobarkar | 244101040 |
| Rahul | 244101035 |

---

## Project Overview

The Entry Exit Face Identification Door Lock System is designed to:

- **Identify authorized personnel** using advanced face recognition algorithms
- **Track entry and exit** of individuals in real-time
- **Provide secure access control** without physical contact
- **Log activity** for security monitoring and analysis
- **Use object detection** for enhanced security features

## Key Features

- **Real-time Face Detection & Recognition** using state-of-the-art algorithms
- **Automated Door Lock Control** based on identity verification
- **Entry/Exit Logging** with timestamp and identity tracking
- **Live Video Processing** for continuous monitoring
- **YOLOv5 Integration** for robust object detection
- **User-friendly Interface** for system administration
- **High Security** with multiple verification layers

## Technology Stack

### Machine Learning & AI
- **TensorFlow 2.19.0** - Deep learning framework
- **PyTorch 2.6.0** - Neural network development
- **YOLOv5 (Ultralytics)** - Object detection
- **Face Recognition** - Facial identification
- **OpenCV 4.11.0** - Computer vision processing

### Data Processing & Analysis
- **NumPy 2.1.1** - Numerical computations
- **Pandas 2.2.3** - Data manipulation
- **Matplotlib 3.10.1** - Data visualization
- **Seaborn 0.13.2** - Statistical plotting

### Development Environment
- **Jupyter Notebooks** - Interactive development
- **Python 3.x** - Primary programming language

## Project Structure

```
entry-exit-face-identification-door-lock-system/
├── Demo1.ipynb                    # Object detection demonstration
├── Demo2.ipynb                    # Face recognition demo
├── Demo3.ipynb                    # Complete system demo
├── Training.ipynb                 # Model training notebook
├── Testing.ipynb                  # System testing procedures
├── requirements.txt               # Python dependencies
├── IPML_Report.pdf               # Project report
├── content/
│   ├── cropped_image/            # Processed images
│   ├── exp5/                     # Training experiment results
│   │   ├── weights/              # Trained model weights
│   │   │   ├── best.pt
│   │   │   └── last.pt
│   │   ├── confusion_matrix.png
│   │   ├── results.csv
│   │   └── ...                   # Training metrics & plots
│   ├── live_image/               # Live capture samples
│   └── videos/                   # Demo video files
└── setups/                       # Installation files
```

## Getting Started

### Prerequisites

- Python 3.8 or higher
- CUDA-compatible GPU (recommended for faster processing)
- Webcam or IP camera for live detection
- Sufficient storage space for model weights and data

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/saikiran31415/entry-exit-face-identification-door-lock-system.git
cd entry-exit-face-identification-door-lock-system
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Install additional requirements** (if needed)
```bash
# For Tesseract OCR (Windows)
# Run the setup file in setups/ directory

# For face recognition models
pip install dlib cmake
```

### Quick Start

1. **Training the Model**
   - Open `Training.ipynb` in Jupyter
   - Follow the step-by-step training process
   - Model weights will be saved in `content/exp5/weights/`

2. **Testing the System**
   - Run `Testing.ipynb` for system validation
   - Verify face detection and recognition accuracy

3. **Live Demonstration**
   - Execute `Demo1.ipynb` for object detection
   - Run `Demo2.ipynb` for face recognition
   - Use `Demo3.ipynb` for the complete system demo

## Usage

### Basic Operation

1. **Initialize the system** by loading trained models
2. **Configure camera input** (webcam or IP camera)
3. **Start the detection service** for real-time monitoring
4. **Monitor entry/exit logs** through the interface
5. **Manage authorized users** in the system database

### Advanced Features

- **Batch processing** of images for offline analysis
- **Custom training** with new face datasets
- **Integration** with external door lock systems
- **Export logs** for security analysis and reporting

## Model Performance

The system achieves:
- **High accuracy** in face recognition under various lighting conditions
- **Real-time processing** at 30+ FPS on modern hardware
- **Low false positive rate** for enhanced security
- **Robust detection** across different camera angles

Performance metrics and training curves are available in the `content/exp5/` directory.

## Demo Videos

Sample demonstration videos are available in the `content/videos/` directory:
- `20250418_132622.mp4` - System operation demo
- `20250418_132955.mp4` - Face recognition showcase

## Documentation

- **Project Report**: `IPML_Report.pdf` contains detailed technical documentation
- **Code Documentation**: Inline comments and markdown cells in notebooks
- **Training Logs**: Available in `content/exp5/results.csv`

## Contributing

This is an academic project developed by the Game Changers team. For educational purposes and improvements:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
