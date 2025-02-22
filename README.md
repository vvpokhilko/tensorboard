# Project Summary: Experiment Tracking with TensorBoard for PyTorch Vision Models
This project explores **experiment tracking** using **TensorBoard** while training **PyTorch vision models**. The goal is to analyze the impact of different **model architectures**, **data augmentation** and **training duration** on model performance.

## Project Workflow:

### 1. Dataset & Preprocessing:
* Used a subset of the [Food101 dataset](https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/) (20% of the data and 3 classes only - pizza, steak and sushi).
* Applied **TrivialAugmentWide()** for augmentation in one experiment and compared results with non-augmented data.

### 2. Model Selection:
* Trained **EfficientNetB3** and **RegNet_Y_1_6GF**, both available in `torchvision.models`.

### 3. Experiment Setup:

* Conducted eight experiments by varying:
  * Models: **EfficientNetB3** vs. **RegNet_Y_1_6GF**
  * Data Augmentation: **With vs. Without TrivialAugmentWide()**
  * Training Duration: **5 vs. 10 epochs**
* Used **TensorBoard** to log training loss, validation accuracy, and model performance.

### 4. Training & Tracking:

* Logged key metrics (`loss`, `accuracy`) in TensorBoard.
* Compared model convergence, generalization, and improvement with longer training and augmentation.

### 5. Results & Analysis:

* Observed the impact of **augmentation** on accuracy improvements.
* Evaluated whether **longer training (10 epochs) outperforms 5 epochs**.
* Compared performance trends across **EfficientNetB3** and **RegNet_Y_1_6GF**.

## Key Takeaways:
* TensorBoard is effective for **visualizing training dynamics**.
* **Data augmentation** improves generalization, especially for small datasets.
* **Longer training (10 epochs)** can enhance performance but may lead to diminishing returns.
* **EfficientNetB3** vs. **RegNet_Y_1_6GF**: Model efficiency and performance differences were analyzed.

This project demonstrates the power of **experiment tracking** in deep learning workflows, ensuring reproducibility and insights into model performance. 🚀
