# COVID-19 Detection using Chest X-rays and CT Scans

> **Original Project**: This project is based on the work by [Kaushik Jadhav](https://github.com/kaushikjadhav01/COVID-19-Detection-Flask-App-based-on-Chest-X-rays-and-CT-Scans) and has been modified and enhanced for educational purposes.

> **Live Demo**: [Original Project Demo](http://coviddetector.kajadhav.me)

An enhanced version of a comprehensive AI-powered system for detecting COVID-19 from medical imaging using multiple deep learning models. This project implements four state-of-the-art transfer learning algorithms to analyze chest X-rays and CT scans for COVID-19 detection.

**Enhanced Features:**
- Improved documentation and setup instructions
- Better project structure and organization
- Enhanced technical details and usage guidelines
- Proper attribution to original author

## 🚀 Features

- **Multi-Model Analysis**: Uses 4 different deep learning models for robust predictions
- **Dual Imaging Support**: Processes both Chest X-rays and CT Scans
- **High Accuracy**: Achieves up to 96% accuracy on chest X-rays
- **Web Interface**: User-friendly Flask web application
- **Real-time Processing**: Instant results with confidence scores
- **Medical Grade**: Trained on real medical imaging data
- **Enhanced Documentation**: Improved README and setup instructions

## 📊 Model Performance

| Model | Chest X-rays | CT Scans |
|-------|-------------|----------|
| **InceptionV3** | 96% | 93% |
| **VGG16** | 94% | 93% |
| **ResNet50** | 83% | 80% |
| **Xception** | 92% | 95% |

## 🏗️ Architecture

### Deep Learning Models Used:
1. **InceptionV3**: 48-layer CNN with 299x299 input size
2. **VGG16**: 16-layer CNN with 224x224 input size  
3. **ResNet50**: 50-layer residual network with 224x224 input size
4. **Xception**: 71-layer depthwise separable CNN with 299x299 input size

### Technical Stack:
- **Backend**: Flask (Python web framework)
- **AI/ML**: TensorFlow 2.4.1, Keras
- **Image Processing**: OpenCV, NumPy
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap
- **Training**: Google Colab GPU

## 📁 Project Structure

```
Covid-19-Prediction-using-Chest-X-Ray-and-CT-Scan/
├── app.py                          # Main Flask application
├── requirements.txt                 # Python dependencies
├── README.md                       # This file
├── models/                         # Trained model files
│   ├── resnet_chest.h5
│   ├── vgg_chest.h5
│   ├── inceptionv3_chest.h5
│   ├── xception_chest.h5
│   ├── resnet_ct.h5
│   ├── vgg_ct.h5
│   ├── inception_ct.h5
│   └── xception_ct.h5
├── flask app/                      # Web application files
│   ├── index.html                  # Homepage
│   ├── upload.html                 # File upload interface
│   ├── results_chest.html          # Chest X-ray results
│   ├── results_ct.html             # CT scan results
│   ├── about.html                  # About page
│   ├── contact.html                # Contact page
│   ├── faqs.html                   # FAQ page
│   ├── prevention.html             # Prevention guidelines
│   └── assets/                     # CSS, JS, images
├── data/                           # Dataset directory
│   ├── chest/                      # Chest X-ray images
│   └── ct/                         # CT scan images
├── jupyter notebooks/              # Training notebooks
├── python files/                   # Individual model scripts
└── screenshots/                    # Application screenshots
```

## 🛠️ Installation

### Prerequisites
- Python 3.6.9 or higher
- pip package manager

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Devarshi0808/Covid-19-Prediction-using-Chest-X-Ray-and-CT-Scan.git
   cd Covid-19-Prediction-using-Chest-X-Ray-and-CT-Scan
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application:**
   ```bash
   python app.py
   ```

4. **Access the web interface:**
   Open your browser and go to: **http://127.0.0.1:5000**

## 🎯 Usage

### Web Interface
1. **Upload Image**: Select a chest X-ray or CT scan image
2. **Choose Model**: Select from 4 different AI models
3. **Get Results**: Receive instant COVID-19 detection results with confidence scores

### Supported File Formats
- **Images**: PNG, JPG, JPEG, GIF
- **Recommended**: High-quality medical images (224x224 or 299x299 pixels)

## 📈 Dataset Information

### Training Data
- **Chest X-rays**: 1,000 images (800 training, 200 testing)
- **CT Scans**: 750 images (600 training, 150 testing)
- **Split Ratio**: 80% training, 20% testing

### Data Sources
- Medical imaging databases
- Public COVID-19 datasets
- Validated medical images

## 🔬 Technical Details

### Model Training
- **Epochs**: 500 epochs per model
- **Platform**: Google Colab with GPU acceleration
- **Transfer Learning**: Pre-trained on ImageNet
- **Optimization**: Adam optimizer with binary cross-entropy loss

### Image Processing Pipeline
1. **Preprocessing**: Resize to model-specific dimensions
2. **Normalization**: Scale pixel values to [0,1]
3. **Augmentation**: Training data augmentation for robustness
4. **Inference**: Real-time prediction with confidence scores

## 🌐 Web Application Features

### Pages
- **Home**: Overview and navigation
- **Upload**: Image upload interface
- **Results**: Detailed prediction results
- **About**: Project information
- **Contact**: Contact form
- **FAQs**: Frequently asked questions
- **Prevention**: COVID-19 prevention guidelines

### Key Features
- **Responsive Design**: Works on desktop and mobile
- **Real-time Processing**: Instant AI predictions
- **Multiple Models**: Compare different AI approaches
- **Confidence Scores**: Detailed prediction probabilities
- **User-friendly Interface**: Intuitive medical imaging upload

## 📊 Results and Evaluation

### Performance Metrics
- **Accuracy**: Up to 96% on chest X-rays
- **Sensitivity**: High true positive rate
- **Specificity**: Low false positive rate
- **F1-Score**: Balanced precision and recall

### Sample Results
Check the `screenshots/` folder for sample predictions and interface examples.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Authors

### Original Author
**Kaushik Jadhav**
- GitHub: [kaushikjadhav01](https://github.com/kaushikjadhav01)
- Portfolio: [kajadhav.me](http://kajadhav.me/)
- Medium: [@kaushikjadhav01](https://medium.com/@kaushikjadhav01)
- LinkedIn: [kaushikjadhav01](https://www.linkedin.com/in/kaushikjadhav01/)

### Enhanced Version
**Devarshi0808** - Enhanced documentation and improvements

## 🙏 Acknowledgments

### Original Project
- **Kaushik Jadhav** - Original implementation and research
- **Towards Data Science** - [Published Article](https://towardsdatascience.com/covid-19-detector-flask-app-based-on-chest-x-rays-and-ct-scans-using-deep-learning-a0db89e1ed2a)

### Technical Acknowledgments
- Medical imaging datasets and research community
- TensorFlow and Keras development teams
- Flask web framework community
- Healthcare professionals for validation

## ⚠️ Disclaimer

This tool is for research and educational purposes only. It should not be used as a substitute for professional medical diagnosis. Always consult healthcare professionals for medical decisions.

---

## 📋 Project Status

This is an enhanced version of the original COVID-19 Detection project by Kaushik Jadhav. The core functionality and models remain the same, but the documentation and setup instructions have been improved for better user experience.

### Modifications Made:
- ✅ Enhanced README with comprehensive documentation
- ✅ Improved installation instructions
- ✅ Better project structure documentation
- ✅ Added proper attribution to original author
- ✅ Enhanced technical details and usage guidelines

**Note**: This project demonstrates the potential of AI in medical imaging but should be used responsibly and in conjunction with professional medical expertise.





