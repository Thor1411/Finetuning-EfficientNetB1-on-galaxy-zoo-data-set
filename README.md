# Galaxy Morphology Classification using EfficientNet-B1 and LoRA

This project focuses on finetuning a pre-trained EfficientNet-B1 model to classify galaxy images from the Galaxy Zoo 2 dataset. Additionally, the project explores the use of LoRA (Low-Rank Adaptation) to enhance the finetuning process by reducing the number of trainable parameters and computational cost.

---

## Project Structure

- `Notebook.ipynb`: Main notebook performing data preprocessing, model finetuning, and evaluation.
- `training_solutions_rev1.csv`: Labels containing galaxy morphology information.
- `images/`: Folder containing galaxy images (`GalaxyID.jpg`).

---

## Objective

To classify galaxies based on their morphology by:

1. Finetuning a pre-trained EfficientNet-B1 model.
2. Comparing traditional finetuning vs LoRA-based finetuning.
3. Evaluating the effectiveness of LoRA in terms of performance and efficiency.

---

## Methodology

### Model: EfficientNet-B1

- A lightweight yet powerful convolutional neural network.
- Pretrained on ImageNet and adapted to the galaxy classification task.

### LoRA (Low-Rank Adaptation)

- Injects low-rank matrices into pretrained weights to make only a subset trainable.
- Reduces memory footprint and accelerates training without compromising performance.

---

## Dataset

- Source: Galaxy Zoo 2 project (https://data.galaxyzoo.org/)
- Images: Each image represents a galaxy identified by `GalaxyID`.
- Labels: A CSV file contains answers to morphology-related questions (e.g., spiral, smooth, edge-on).

---

## Setup

### Dependencies

```bash
pip install torch torchvision pandas numpy matplotlib timm peft
