<div align="center">

#  [Group H] Custom CNN for Banana Classification & Ripeness Detection
### A Deep Learning Assignment for CSE366

</div>

---

##  Project Overview

This project demonstrates deep learning craftsmanship by designing, training, and evaluating two novel Convolutional Neural Networks (CNNs) from scratch. The models are built to solve two distinct computer vision tasks using a comprehensive dataset of bananas from Bangladesh:

1.  **Variety Classification:** Identifying the specific variety of a banana (e.g., Sagor Kola, Champa Kola).
2.  **Ripeness Detection:** Determining the ripeness stage of a banana (e.g., Green, Ripe, Overripe).

The entire workflow, from data analysis to model benchmarking, is documented in the accompanying Kaggle notebooks.

---

##  Group Members

| Name                | ID              |
| ------------------- | --------------- |
| **Khalid Mahmud Joy** | `2022-3-60-159` |
| **Shahriar Khan** | `2022-3-60-016` |
| **Tanvir Rahman** | `2022-3-60-134` |
| **Rifah Tamannah** | `2022-3-60-149` |

---

##  Key Features & Technical Rigour

* **Novel CNN Architectures:** Two unique CNNs, `BANANA_CLASS_CNN` and `BANANA_RIPE_CNN`, were designed and built from scratch with 6 convolutional blocks each.

* **Overfitting Analysis:** We demonstrate the ability to monitor overfitting by training a baseline model and then solve it using advanced regularization techniques.

* **Advanced Training Pipeline:** The models are trained using a professional pipeline that includes:
    * **Mixed Precision Training** (`torch.cuda.amp`) for significant speed-ups.
    * **Data Augmentation** (`TrivialAugmentWide`) to improve model generalization.
    * **Early Stopping** and **LR Scheduling** (`CosineAnnealingWarmRestarts`) for efficient training.

* **Comprehensive Benchmarking:** Our custom models are evaluated against 5 state-of-the-art pre-trained models, including `ResNet50`, `VGG16`, and `EfficientNet-B0`.

* **In-depth Visualization:** The notebooks include detailed data visualizations, performance graphs, and confusion matrices for every model.

---

##  How to Reproduce

1.  **Environment:** Open the project in a Kaggle Notebook environment with a **GPU accelerator** enabled (T4 x2 recommended).

2.  **Dataset:** Add the dataset by searching for its Kaggle URL:
    ```
    [https://data.mendeley.com/datasets/ptfscwtnyz/2]
    ```
    > **Note:** *Ensure the input directory in the notebook matches `/kaggle/input/banana-image-bd/...`*

3.  **Execution:** Upload the `BananaImage_Banana_Class_Ripeness_Detection_BD.ipynb` notebook file.

4.  **Run All:** Execute all cells from top to bottom. The notebook is self-contained and will:
    * Perform all data analysis and visualization.
    * Train the baseline model to show overfitting.
    * Train and evaluate the final 6 models for each task.
    * Generate the final comparison tables.
