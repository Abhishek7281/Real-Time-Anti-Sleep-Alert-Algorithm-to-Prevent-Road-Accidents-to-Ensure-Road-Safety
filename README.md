# Real-Time-Anti-Sleep-Alert-Algorithm-to-Prevent-Road-Accidents-to-Ensure-Road-Safety

# Project Overview

The Real-Time Anti-Sleep Alert Algorithm is designed to prevent road accidents caused by driver drowsiness. It employs deep learning models to detect signs of drowsiness in real-time and alerts the driver through an alarm system. The solution is optimized for embedded systems such as Raspberry Pi, ensuring portability and efficiency for real-world applications.


# Features

1. Real-time driver drowsiness detection using deep learning models.

2. High accuracy detection using InceptionV3, VGG16, and MobileNetV2.

3. Facial landmark detection to analyze eye state and compute the Eye Aspect Ratio (EAR).

4. Non-invasive monitoring through a web camera.

5. Embedded system deployment using Raspberry Pi 4B.

6. Immediate alerts via buzzer to warn drowsy drivers.



# Methodology

The system follows these steps:

1. Image Acquisition: Captures real-time video of the driver’s face using a web camera.

2. Face & Eye Detection: Detects facial landmarks and eye status (open/closed).

3. Deep Learning Model Processing: Uses CNN-based models (InceptionV3, VGG16, MobileNetV2) to classify eye states.

4. Drowsiness Assessment: Computes EAR and identifies drowsiness based on threshold values.

5. Alert Mechanism: Triggers a buzzer alarm if drowsiness is detected for a specific duration.


# Model Training & Performance

The system is trained on the MRL Eye Dataset, consisting of 84,898 images of open and closed eyes. Models were trained and evaluated based on:

1. Accuracy: InceptionV3 (99.18%), VGG16 (98.80%), MobileNetV2 (99.01%)

2. Precision, Recall, and F1-Score

3. Confusion Matrix for validation

#Hardware Requirements

1. Raspberry Pi 4B

2. USB Web Camera (e.g., Logitech HD Webcam C270)

3. Buzzer for alert system

4. Power supply (USB-C or vehicle power)

5. MicroSD card for storage


# Software Requirements

  1. Python 3.7+
  
  2. OpenCV
  
  3. TensorFlow/Keras
  
  4. NumPy
  
  5. Matplotlib
  
  6. dlib (for facial landmark detection)

# Installation & Setup

1. Clone the repository:
    git clone https://github.com/your-repo/real-time-drowsiness-detection.git
cd real-time-drowsiness-detection

2. Install dependencies:
    pip install -r requirements.txt

3. Run the application:
    python drowsiness_detection.py
# Usage

1. The system will continuously monitor the driver’s face.

2. If drowsiness is detected (closed eyes for a prolonged period), an alert will be triggered.

3. The system operates locally on Raspberry Pi, ensuring real-time processing and privacy.
   
# Future Enhancements

1. Improved robustness against extreme weather conditions.

2. Integration with vehicle control systems for automatic speed reduction.

3. Adaptive alert mechanisms, including vibrations and voice warnings.
   
# Contributors

1. Abhishek Kumar Pathak (IIT Indore)

2. Ankit Kumar Singh (Motihari College of Engineering)

3. Pankaj Kumar (Vaishali Engineering College)

4. Vimal Bhatia (IIT Indore, Skoda Auto University)

5. Ondrej Krejcar (Malaysia Japan International Institute of Technology)

# Acknowledgments

This research is supported by SERB, DST, Government of India (CRG/2021/001215) and Skoda Auto University.

# License

This project is licensed under the MIT License - see the LICENSE file for details.

