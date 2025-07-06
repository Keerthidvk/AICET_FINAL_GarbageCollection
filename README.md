🧠 Smart Garbage Classification with Deep Learning

Let’s face it—waste segregation can be a real mess. So why not let AI handle the dirty work? This project uses deep learning to automatically classify garbage images into categories like plastic, paper, metal, and more, making recycling smarter, faster, and more efficient. ♻️

🌟 What’s Inside

🔍 A powerful image classifier built on EfficientNetV2B2
🧱 Custom classification layers tuned for trash detection
🖼️ Gradio interface to test images in real-time — just drag, drop, and predict!
📊 Visual insights with confusion matrices and heatmaps
🧠 Clean, modular code that’s easy to understand and expand

🧰 Tech Stack

 Python 
 TensorFlow / Keras for model building and training
 EfficientNetV2B2 – transfer learning that packs a punch
 scikit-learn for metrics and reports
 matplotlib + seaborn for visualization
 Gradio for the interactive UI
 Jupyter Notebook for development and experimentation

📂 The Dataset

The model is trained on a curated dataset of labeled trash images, resized to 124×124 pixels for consistency
🧪 Split: 80% for training, 20% for validation
📦 Loaded using image_dataset_from_directory in TensorFlow

🛠️ How It Works

Data Preparation
The images are resized, batched, shuffled, cached, and prefetched for performance.

Model Building
EfficientNetV2B2 serves as the backbone. On top, we’ve added dropout layers and dense layers to fine-tune it for garbage classification.

Training

Optimizer: Adam
Loss Function: Categorical Crossentropy
Callbacks: EarlyStopping, ReduceLROnPlateau to avoid overfitting

Evaluation
The model is evaluated using a confusion matrix, classification report, and visual performance plots.

Deployment
Everything is wrapped up in a clean Gradio app so you can classify trash images right from your browser!
