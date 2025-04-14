# 🦴 Fractured, Or Not-Fractured — That Is The Question  
### An Image Processing and Computer Vision Project | Ironhack Data Science Bootcamp

## 📌 Introduction  
Computer vision is a powerful application of deep learning that enables machines to interpret and understand visual data. In this project, I applied a computer vision approach to classify bone X-ray images into two categories: **fractured** and **non-fractured**. These X-rays come from various body parts, offering a diverse dataset for training and evaluation. The primary objective was to utilize a modern deep learning model to automate fracture detection, a task with significant potential in medical diagnostics.

## 🎯 Project Goals  
- ✅ Preprocess the dataset by splitting it into **training**, **validation**, and **test** sets.  
- ✅ Apply **data augmentation** techniques (e.g., image flipping and rotation) to increase model generalizability.  
- ✅ Use a **pre-trained state-of-the-art model** (Transfer Learning) for efficient and accurate classification.  
- ✅ Evaluate model performance using **accuracy metrics** and **confusion matrix**.  
- ✅ Prepare a clear and concise **presentation** for stakeholders.

## 📂 Data Source  
- **Bone Fracture X-ray Dataset**  
  📎 [Download here](https://drive.google.com/file/d/1WeuxOenviI1_ElW5ISED4MhvR_YFYdmB/view?usp=drive_link)  
  This dataset consists of X-ray images from various regions of the body, labeled as fractured or non-fractured.

## ⚙️ Methodology  
1. **Data Cleaning**:  
   - Removed corrupted or unreadable images using `TensorFlow` utilities.  

2. **Model Architecture**:  
   - Used `MobileNetV2` (a lightweight, efficient CNN model) as the backbone for classification.  
   - Applied transfer learning by fine-tuning only the top layers to adapt to our specific classification task.

3. **Training Setup**:  
   - Trained for **30 epochs** with early stopping based on validation loss.  
   - Saved the best performing model as `best_model.keras`.  

4. **Evaluation**:  
   - Assessed model performance using **accuracy**, **loss curves**, and a **confusion matrix**.

## 💡 Key Insights  
- `MobileNetV2` achieved a high classification **accuracy of 96%**.  
- The model showed **minimal Type I and Type II errors**, making it highly reliable.  
- Transfer learning significantly improved efficiency and performance, even with a moderately sized dataset.

## 🧾 Project Structure  
```bash
fracture-classifier/
│
├── data/                 # Download and keep your data here
├── code/                 # Jupyter Notebooks for EDA, training and evaluation, best model (.keras) is here
├── presentation/         # Presentation to the stakeholder 
├── README.md             # Project documentation (this file)
├── task.md               # Task given in the project 
└── requirements.txt      # Python dependencies
```

## 🚀 Getting Started
1. Clone the repository
   ```bash
   git clone https://github.com/abhishek-chattopadhyay/project-4-cv.git
   cd project-4-cv
   ```
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Download the data from the link and put it into the data folder.
4. Run the `main.ipynb`

## 📝 Extra Notes
- This project was developed as part of the Ironhack Data Science Bootcamp.
- Future enhancements could include:
  - Trying other models like EfficientNet, ResNet, or ensemble techniques.
  - Expanding the dataset to include more fracture types.
  - Deploying the model via a simple web app for demo purposes.
