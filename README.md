🥔🍅🥬 Ninjacart Vegetable Image Classification using CNN & Transfer Learning

📝 Problem Statement
Ninjacart, India's largest fresh produce supply chain company, automates quality checks using AI models that classify vegetables in real-world market scenes. The goal of this project is to develop a robust multi-class image classifier that can identify Onion, Potato, Tomato, and Noise (non-vegetable/market scenes) using a custom dataset scraped from the internet.

📦 Dataset
The dataset is provided by Ninjacart and consists of images scraped from Google.

It contains train/ and test/ folders with 4 subfolders: tomato, potato, onion, and indian market (noise).

🔢 Dataset Distribution:
Train Folder:

Tomato: 789 images

Potato: 898 images

Onion: 849 images

Indian Market (Noise): 599 images

Test Folder:

Tomato: 106 images

Potato: 83 images

Onion: 81 images

Indian Market (Noise): 81 images

📎 Download Dataset from Google Drive

🧠 Concepts Implemented
Data Preprocessing & Augmentation

Exploratory Data Analysis & Visualization

Convolutional Neural Networks (CNNs)

Overfitting Handling (Dropout, BatchNormalization)

Callbacks (EarlyStopping, ModelCheckpoint, TensorBoard)

Transfer Learning using VGG16, ResNet50, MobileNet

Confusion Matrix and Classification Report

⚙️ Project Workflow
1. 📥 Data Preparation
Downloaded and extracted data using gdown

Checked image dimensions and class distribution

Visualized random samples using matplotlib

Verified folder-wise image counts

Resized all images to 224x224 and normalized pixel values

Split dataset into 80% training and 20% validation

2. 📊 Exploratory Data Analysis
Plotted class distribution using seaborn

Displayed sample images from each class

Validated non-uniformity in image shapes

3. 🧱 Model Development
✅ Baseline CNN Model:
Built from scratch using Conv2D, MaxPooling, Dropout, Dense

Optimized using Adam optimizer, categorical_crossentropy

🔁 Transfer Learning:
Implemented with VGG16, ResNet50, and MobileNet

Used pretrained weights on ImageNet

Fine-tuned top layers

Compared performance using accuracy and confusion matrix

4. 📉 Handling Overfitting
Applied Dropout, BatchNormalization

Used EarlyStopping, ModelCheckpoint, ReduceLROnPlateau

Performed real-time image augmentation using ImageDataGenerator

5. 📈 Evaluation
Plotted training and validation accuracy/loss graphs

Generated confusion matrix

Evaluated final model on the test set

Performed predictions on random sample images

📊 Results
Achieved >90% accuracy on test data with ResNet50 + Augmentation + Fine-tuning

Model successfully distinguished vegetable types and filtered noisy market scenes

Helped simulate real-world quality control scenario in agri-supply chain
