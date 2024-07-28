# Lightweight Convolutional Neural Networks for Diabetic Retinopathy Detection using Knowledge Distillation

## Abstract

Diabetic Retinopathy (DR) is a serious consequence of diabetes, posing a significant threat to vision and potentially leading to irreversible blindness if not diagnosed early. It generally impacts 80% of people who have had diabetes for more than 10 years. This condition arises from diabetes-induced damage to retinal blood vessels, emphasizing the critical need for precise and timely intervention and diagnosis. Traditional screening methods depend on the manual examination of colored fundus images by trained specialists, which can be prone to errors, potentially missing early signs of diabetic retinopathy.

To address this challenge, various Convolutional Neural Networks (CNNs) such as DenseNet121, DenseNet169, DenseNet201, MobileNet, ResNet152, Xception, and Inception have been explored. Through rigorous experimentation, we meticulously engaged with these models to examine their capabilities to enhance the precision of DR diagnosis in all its stages. Though these models provide decent accuracies, their size makes them complex to embed in miniature medical devices.

In this paper, we introduce the application of Knowledge Distillation by implementing a teacher-student model. Our research aims to achieve a lighter, more compact, and simpler student model derived from the more complex teacher models. After thorough analysis, we found that the student model mentored by DenseNet169 outshines other models, accurately detecting Diabetic Retinopathy (DR) with the highest validation accuracy of 68.77%. Using a diverse dataset from Kaggle, our focus goes beyond just improving accuracy; we aim to contribute valuable insights to the fight against this sight-threatening diabetes complication.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Models](#models)
- [Knowledge Distillation](#knowledge-distillation)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Diabetic Retinopathy (DR) is a severe complication of diabetes, often leading to blindness if not detected and treated early. Traditional diagnostic methods involve manual examination of retinal images, which can miss early signs of DR. To improve the accuracy and efficiency of DR diagnosis, we explore the use of Convolutional Neural Networks (CNNs) and Knowledge Distillation to develop a lightweight model suitable for deployment in medical devices.

## Dataset

The dataset used for this research is sourced from Kaggle, containing diverse images of retinal scans. The dataset is preprocessed and split into training, validation, and test sets to ensure robust model evaluation.

You can download the dataset using the following Kaggle API key:
```
kaggle datasets download -d sachinkumar413/diabetic-retinopathy-dataset
```

## Models

We have explored various CNN architectures, including:
- DenseNet121
- DenseNet169
- DenseNet201
- MobileNet
- ResNet152
- Xception
- Inception

## Knowledge Distillation

Knowledge Distillation is a technique where a smaller, simpler student model is trained to replicate the behavior of a larger, more complex teacher model. In this research, DenseNet169 serves as the teacher model, guiding the student model to achieve high accuracy with a reduced model size.

## Results

The student model, distilled from DenseNet169, achieved the highest validation accuracy of 68.77%. This compact model demonstrates the potential for effective DR diagnosis while being suitable for deployment in resource-constrained environments.

## Installation

To install the necessary dependencies, run:

```bash
pip install -r requirements.txt
```

## Usage

To train and evaluate the models, follow these steps:

1. Clone the repository:
    ```bash
    `git clone` https://github.com/FRAGGERR/Diabetic-Retinopathy.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Diabetic-Retinopathy
    ```
3. Run the training script:
    ```bash
    python train.py
    ```

## Contributing

We welcome contributions to improve the project. Please submit a pull request or open an issue for any suggestions or improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to modify or clone the repo, (Contact info. ``` hardikchhipa28@gmail.com```).

