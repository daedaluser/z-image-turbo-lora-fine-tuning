Z-Image-Turbo Training & Inference Toolkit
A comprehensive toolkit for LoRA fine-tuning and inference with Z-Image-Turbo - a high-speed image generation model.
Quick Start
1. Clone Repository
git clone https://github.com/[username]/z-image-turbo.git
cd z-image-turbo
2. Setup Environment
# Install dependencies
pip install -r requirements.txt

# Or use conda
conda env create -f environment.yml
conda activate z-image-turbo
3. File Structure Setup
Download the training and inference notebooks from this repository and place them in the following structure:
Z-image/
├── src/
│   ├── zimage-lora.ipynb      # LoRA fine-tuning notebook
│   └── infer_lora.ipynb        # LoRA inference notebook
├── ...
3. Workflow:
Prepare your dataset (images in data/train/)
Configure hyperparameters (rank, learning rate, epochs)
Run all cells to start training
Find checkpoints in outputs/lora/
