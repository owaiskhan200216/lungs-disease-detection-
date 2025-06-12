# 🫁 Lung Disease Detection from Chest X-ray Images

An intelligent healthcare application that uses deep learning to detect five lung diseases from X-ray images, along with location-based hospital recommendations and an interactive chatbot for patient guidance.

---

## 🚀 Features

- 🎯 **Disease Detection**: Classifies chest X-rays into:
  - Bacterial Pneumonia  
  - COVID-19  
  - Normal  
  - Tuberculosis  
  - Viral Pneumonia

- 🖼️ **CustomTkinter GUI**:
  - User registration & login
  - Real-time X-ray upload and prediction
  - Prediction history tracking

- 🗺️ **Geolocation & Hospital Finder**:
  - Uses OpenCage Geocoding & Geopy to fetch user location
  - Recommends and maps nearby hospitals using Folium

- 🤖 **Integrated Chatbot**:
  - Responds to queries about symptoms, treatments, and prescriptions
  - Pulls information from a structured MySQL disease database

---

## 🧠 Model Details

- **Architecture**: Xception CNN (ImageNet pre-trained)
- **Framework**: TensorFlow / Keras
- **Input Size**: 299 × 299 × 3
- **Loss Function**: Categorical Crossentropy
- **Optimizer**: Adam
- **Data Augmentation**: Rotation, shift, zoom, flip

---

## 🗃️ Dataset

- NIH Chest X-ray Dataset
- Preprocessed and augmented locally
- Class imbalance handled via oversampling & augmentation

---

## 💻 Tech Stack

| Component     | Technology             |
|---------------|------------------------|
| Deep Learning | TensorFlow, Keras      |
| GUI           | CustomTkinter          |
| Geolocation   | OpenCage API, Geopy    |
| Mapping       | Folium, Webbrowser     |
| Database      | MySQL                  |
| NLP Logic     | Rule-based Python bot  |
| Image Handling| Pillow (PIL)           |

---

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/lung-disease-detection.git
cd lung-disease-detection



2. Install dependencies:


pip install -r requirements.txt

3. Set up your MySQL database:

Import schema.sql for users, history, hospitals, and diseases.
Update DB credentials in db_connector.py.

4. Run the application:

python app_gui.py

5. 🔑 API Keys Required
OpenCage Geocoding API
Get your key from: https://opencagedata.com
Add it in the script:
API_KEY = "your_opencage_api_key"


6. 📚 License
This project is licensed under the MIT License. 
