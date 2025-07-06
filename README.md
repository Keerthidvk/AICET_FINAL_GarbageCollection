# 🗑️ Garbage Classification with Deep Learning

This project is about building an AI-based system to automatically classify garbage images into different categories, like plastic, metal, paper, etc. The goal is to make waste segregation smarter and faster, supporting better recycling practices.

## 🌟 What’s Inside
- A deep learning model based on **EfficientNetV2B2**
- Custom layers on top for trash classification
- Gradio interface for easy, real-time image predictions
- Visual performance reports using confusion matrix and heatmaps
- Code that’s simple and easy to extend

## 🔧 Tech Stack
- **Python**
- **TensorFlow / Keras**
- **EfficientNetV2B2** (transfer learning)
- **scikit-learn**
- **matplotlib + seaborn** (for charts)
- **Gradio** (for the interactive interface)
- **Jupyter Notebook**

## 📂 Dataset
The model was trained on an image dataset of various trash types.  
- Images resized to 124×124 pixels  
- Data split: 80% training, 20% validation  
- Loaded using TensorFlow’s `image_dataset_from_directory`  

## 📝 How It Works
1. **Load and prepare the data**  
   Resize, batch, shuffle, cache, and prefetch the dataset.

2. **Build the model**  
   Use EfficientNetV2B2 as a base, add dropout and dense layers for classification.

3. **Train the model**  
   Optimizer: Adam  
   Loss: Categorical crossentropy  
   Callbacks: EarlyStopping, ReduceLROnPlateau  

4. **Evaluate performance**  
   Generate confusion matrix, classification report, and plots.

5. **Deploy**  
   Serve predictions through a simple Gradio web app.


