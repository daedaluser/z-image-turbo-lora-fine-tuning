Z-Image-Turbo Training & Inference Toolkit
A comprehensive toolkit for LoRA fine-tuning and inference with Z-Image-Turbo - a high-speed image generation model.
Quick Start
1. Clone Repository
bash
复制
git clone https://github.com/[username]/z-image-turbo.git
cd z-image-turbo
2. Setup Environment
bash
复制
# Install dependencies
pip install -r requirements.txt

# Or use conda
conda env create -f environment.yml
conda activate z-image-turbo
3. File Structure Setup
Download the training and inference notebooks from this repository and place them in the following structure:
复制
z-image-turbo/
├── src/
│   ├── zimage-lora.ipynb      # LoRA fine-tuning notebook
│   └── infer_lora.ipynb        # LoRA inference notebook
├── models/                     # Model checkpoints directory
├── data/                       # Training data
└── outputs/                    # Training outputs & logs
Quick Setup Command:
bash
复制
# Assuming you've cloned this tools repo
cp zimage-lora.ipynb z-image-turbo/src/
cp infer_lora.ipynb z-image-turbo/src/
cd z-image-turbo/src
Usage
🎓 Training (LoRA Fine-tuning)
Open zimage-lora.ipynb in Jupyter Lab/Notebook:
bash
复制
jupyter lab zimage-lora.ipynb
Workflow:
Prepare your dataset (images in data/train/)
Configure hyperparameters (rank, learning rate, epochs)
Run all cells to start training
Find checkpoints in outputs/lora/
🚀 Inference
Open infer_lora.ipynb:
bash
复制
jupyter lab infer_lora.ipynb
Workflow:
Load base Z-Image-Turbo model
Load your trained LoRA weights
Generate images with custom prompts
Requirements
Python 3.8+
PyTorch 2.0+
CUDA 11.7+ (for GPU acceleration)
Transformers, Diffusers, PEFT
Jupyter Notebook/Lab
