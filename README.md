🧠 Dynamic Attribute-Aware Face Sketch Synthesis (DAAFSS)
This repository contains the implementation of Dynamic Attribute-Aware Face Sketch Synthesis (DAAFSS) using deep learning techniques. The architecture is designed for forensic applications, synthesizing accurate and detailed face sketches from photographs using both visual and semantic cues.

📁 Project Structure
bash
Copy
Edit
.
├── daafss-notebook.ipynb     # Main notebook for training and inference
├── README.md                 # Project overview and usage guide
└── assets/                   # (Optional) folder for results or images
🚀 Features
Attribute-guided sketch generation using CLIP and MobileNetV3.

Coarse-to-fine sketch synthesis via U2Net and custom refinement generator.

Multimodal fusion using attention mechanisms.

Losses: adversarial, perceptual (VGG), and cycle-consistency.

🏗️ Model Architecture
Text Encoder: CLIP (OpenAI)

Image Encoder: MobileNetV3

Multimodal Fusion: Attribute Attention

Sketch Generator:

Coarse Stage: U2Net

Refinement Stage: Residual & Dilated Residual Blocks

Discriminator: Spectral Normalized Convolutional Discriminator

📦 Dependencies
bash
Copy
Edit
pip install torch torchvision torchaudio
pip install transformers
pip install opencv-python
pip install matplotlib
pip install scikit-image
Also make sure to download CLIP weights via openai/CLIP.

📝 Usage
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/your-username/daafss.git
cd daafss
2. Run the notebook
Open daafss-notebook.ipynb in Jupyter and follow the cells for:

Loading dataset

Preprocessing

Model training

Inference and sketch synthesis

3. Dataset
Use paired image and sketch data with optional caption/attribute information. Adjust dataset paths inside the notebook accordingly.
