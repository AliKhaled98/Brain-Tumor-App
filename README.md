# Brain-Tumor-App

Brain Tumor Classification & Segmentation Web App
This project is a full-stack AI-powered Flask web application that allows users to **upload brain MRI images** and receive:

-  **Classification**: Determines whether the brain MRI shows signs of a tumor.
-  **Segmentation**: Highlights the exact tumor region in the image (if present).

# Project Features

- Built with **TensorFlow/Keras** and **Flask**
- Frontend styled with **HTML/CSS** and Bootstrap
- Deep Learning models trained on:
  - **Classification**: [Brain MRI Images for Brain Tumor Detection](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection)
  - **Segmentation**: [LGG MRI Segmentation Dataset](https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation)
- Live preview of results (input, prediction, segmented mask)
- Modular folder structure (static, templates, models)


# Model Training

Notebooks for training (Classification.ipynb and Segmentation.ipynb) are included.
U-Net was used for segmentation with augmentation.
ResNet50 used as feature extractor for classification.

# Project Structure
├── app.py # Flask app
├── models/ # Pre-trained Keras models
│ ├── classification_model.keras
│ └── segmentation_model.keras
├── static/ # CSS / image assets
├── templates/ # HTML templates
├── requirements.txt # All required dependencies
├── Classification.ipynb # Classification training notebook
├── Segmentation.ipynb # Segmentation training notebook


---

## How to Run the App Locally

1. Clone the Repository

git clone https://github.com/your-username/brain-tumor-flask-app.git
cd brain-tumor-flask-app

2. Set up the Python Environment

pip install -r requirements.txt

3. Download the Pretrained Models
Download the .keras model files from the  GitHub Releases page.

Extract them into the models/ folder like this:
models/
├── classification_model.keras
└── segmentation_model.keras

4. Run the App
   
python app.py
