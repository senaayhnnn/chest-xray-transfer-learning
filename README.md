# Chest X-ray Transfer Learning

This project focuses on binary classification of chest X-ray images into **Normal** and **Pneumonia** classes using transfer learning.

## Dataset

The dataset contains **200 chest X-ray images** from two classes:

- Normal
- Pneumonia

The dataset was divided into:

- **Training:** 112 images
- **Validation:** 28 images
- **Test:** 60 images

The dataset was prepared in a balanced structure for the classification experiments.

## Models and Experiments

Four different experiments were performed:

1. **ResNet50 Baseline**
2. **ResNet50 with Data Augmentation**
3. **ResNet50 with Fine-Tuning**
4. **DenseNet121**

Pre-trained models were used to benefit from transfer learning.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

## Results

| Experiment | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| ResNet50 Baseline | 96.67% | 100.00% | 93.33% | 96.55% | 94.78% |
| ResNet50 + Data Augmentation | 80.00% | 100.00% | 60.00% | 75.00% | 97.89% |
| ResNet50 + Fine-Tuning | 95.00% | 100.00% | 90.00% | 94.74% | 98.33% |
| DenseNet121 | 75.00% | 100.00% | 50.00% | 66.67% | 98.33% |

## Conclusion

Among the evaluated approaches, the **ResNet50 baseline model achieved the best overall classification performance**, with 96.67% accuracy and 96.55% F1-score.

Although the fine-tuned ResNet50 and DenseNet121 models achieved high ROC-AUC values, their overall accuracy and recall were lower than the baseline model. Data augmentation also reduced the overall classification performance in this experiment.

Therefore, the **pre-trained ResNet50 baseline model** was considered the most suitable approach for this dataset.

## Project Structure

```text
chest-xray-transfer-learning/
│
├── README.md
└── Deep_Learning_Based_Chest_X_Ray_Classification.ipynb
