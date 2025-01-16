# Finetuning-EfficientNetB1-on-galaxy-zoo-data-set

This project fine-tunes the EfficientNet-B1 model on the Galaxy Zoo dataset for galaxy classification into categories like elliptical, spiral, and irregular. The workflow includes data preprocessing, dataset stratification into training, validation, and test sets, and implementation of a custom PyTorch dataset class. LoRA (Low-Rank Adaptation) is applied for efficient fine-tuning, and the model is trained and evaluated using metrics such as accuracy and classification reports, with visualizations for sample predictions.
