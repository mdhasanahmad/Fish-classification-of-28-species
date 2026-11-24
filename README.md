# 🐟 A ConvNeXt-GCN Based Deep Learning Framework for Recognizing Freshwater Fish Species in Bangladesh

<p align="center">
  <b>Intelligent Fish Species Recognition Through Convolutional Feature Learning and Graph-Based Representation</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Deep%20Learning-ConvNeXt--GCN-blue" />
  <img src="https://img.shields.io/badge/Computer%20Vision-Fish%20Recognition-green" />
  <img src="https://img.shields.io/badge/Species-28-orange" />
  <img src="https://img.shields.io/badge/Framework-PyTorch-red" />
  <img src="https://img.shields.io/badge/Research-Computer%20Vision-purple" />
</p>

## 📖 Overview

Bangladesh is home to a remarkable diversity of freshwater fish species, making fish identification an important task for fisheries management, biodiversity conservation, and sustainable aquaculture. However, conventional fish identification approaches often depend on manual observation and expert knowledge, which can be time-consuming, subjective, and difficult to scale.

To address these challenges, this research introduces a **ConvNeXt-GCN-based deep learning framework** for automated recognition of freshwater fish species in Bangladesh.

The proposed framework integrates the powerful visual feature extraction capabilities of **ConvNeXt-Tiny** with the relational representation learning capabilities of **Graph Convolutional Networks (GCNs)**. Rather than relying exclusively on conventional image-based feature learning, the framework incorporates graph-based representations to explore relationships among extracted visual features.

The proposed approach aims to provide a robust and intelligent solution for recognizing **28 freshwater fish species** from digital images.

## ✨ Key Contributions

- **Hybrid Deep Learning Architecture:** Integrates ConvNeXt-Tiny and Graph Convolutional Networks into a unified fish recognition framework.
- **Graph-Based Feature Representation:** Generates graph representations from extracted visual information to capture relationships between feature nodes.
- **Automated Fish Recognition:** Enables image-based identification of freshwater fish species.
- **Bangladesh-Focused Research:** Addresses freshwater fish species recognition in the context of Bangladesh.
- **Publicly Available Dataset:** Presents a collected freshwater fish image dataset containing 28 species, made publicly accessible through Mendeley Data.
- **Comparative Evaluation:** Evaluates the proposed framework against established deep learning architectures.
- **Statistical Significance Analysis:** Employs the Wilcoxon signed-rank test to investigate whether the observed performance improvements are statistically significant.
- **Practical Application Potential:** Supports future development of intelligent fish identification systems for fisheries, aquaculture, and biodiversity monitoring.

## 📊 Dataset Collection and Public Availability

For this research, we collected and developed a freshwater fish image dataset representing **28 distinct fish species found in Bangladesh**. The dataset was assembled to support automated fish species recognition using deep learning and computer vision techniques.

The collected images represent different freshwater fish categories, providing visual information for learning species-specific characteristics such as body morphology, color patterns, texture, and structural variations.

To promote research reproducibility and facilitate further investigation in freshwater fish recognition, the collected dataset has been made publicly available through **Mendeley Data**.

**Dataset Repository:**  
[https://data.mendeley.com/datasets/97vrvc5bf2/1](https://data.mendeley.com/datasets/97vrvc5bf2/1)

### Dataset Summary

| Dataset Property | Description |
|---|---|
| Dataset Domain | Freshwater Fish Recognition |
| Geographic Focus | Bangladesh |
| Dataset Collection | Collected for this research |
| Number of Species | 28 |
| Data Type | Digital Fish Images |
| Learning Task | Multi-Class Image Classification |
| Dataset Availability | Publicly Available |
| Repository | Mendeley Data |
| Deep Learning Backbone | ConvNeXt-Tiny |
| Graph Learning Component | GCN |

The public availability of the dataset is intended to facilitate independent evaluation, comparative studies, and the development of improved automated fish recognition methods.

## 🐠 Samples of the 28 Freshwater Fish Species

The collected dataset contains images from 28 freshwater fish species. Figure 1 presents representative image samples from each class after preprocessing. These samples illustrate the visual diversity across the different fish categories, including variations in body shape, size, color, texture, and morphological characteristics.

The dataset includes species such as Aair, Black Roi, Boal, Chapila, Common Carp, DeshiPuti, Foli, Grass Carp, Ilish, KalBaush, Katla, Koi, Magur, Mirror Carp, Mrigel, Nile Telapiya, Pabda, Pangas, Puti, Rui, Shing, Shol, Shorputi, Silver Carp, Taki, Tarabaim, Telapiya, and Tengra.

**Figure 1. Representative preprocessed image samples of the 28 freshwater fish species included in the collected dataset.**

![Representative Samples of 28 Freshwater Fish Species](Figures/fish_samples.png)

## 🧠 Proposed Methodology

The proposed ConvNeXt-GCN framework consists of interconnected components designed to learn discriminative visual representations and their relationships.

### 1. ConvNeXt-Tiny Feature Extraction

ConvNeXt-Tiny serves as the visual feature extraction backbone. It learns meaningful hierarchical representations from input fish images, capturing important characteristics such as body shape, texture, color patterns, and other distinguishing visual features.

### 2. Graph Generation

The extracted visual representations are transformed into graph structures. The graph consists of nodes and their corresponding relationships, providing a relational representation of the learned features.

### 3. Graph Convolutional Network

The generated graph is processed through Graph Convolutional Network layers with ReLU activation. These layers facilitate information propagation between connected nodes and learn discriminative graph-based representations.

### 4. Global Mean Pooling

Global mean pooling aggregates the learned node representations into a compact graph-level feature vector.

### 5. Classification

The resulting representation is passed through fully connected layers, followed by a Softmax activation function to generate class probabilities and predict the corresponding freshwater fish species.

## 🏗️ Architecture

The overall proposed architecture combines convolutional feature extraction with graph-based representation learning.

**Proposed ConvNeXt-GCN Framework:**

![ConvNeXt-GCN Architecture](Figures/figure6.png)

**Complete Research Workflow:**

![Research Workflow](Figures/fishWorkflow.png)

## ⚙️ Model Pipeline

The complete recognition process follows these steps:

1. Collect freshwater fish images.
2. Preprocess the input images.
3. Extract deep visual representations using ConvNeXt-Tiny.
4. Construct graph representations from the extracted features.
5. Apply GCN layers with ReLU activation.
6. Aggregate graph-level information using global mean pooling.
7. Pass the representations through fully connected layers.
8. Apply Softmax for final species classification.

## 📈 Comparative Experimental Results

To evaluate the effectiveness of the proposed ConvNeXt-GCN framework, comparative experiments were conducted against four established deep learning architectures: DenseNet121, MobileNet, InceptionV3, and ResNet50V2.

The models were evaluated using training, validation, and testing accuracy. The reported values include the corresponding intervals presented in the experimental results.

### Performance Comparison

| Model | Training Accuracy (%) | Validation Accuracy (%) | Testing Accuracy (%) |
|---|---:|---:|---:|
| DenseNet121 | 98.12 (97.93–98.30) | 97.18 (96.61–97.75) | 97.22 (96.80–97.63) |
| MobileNet | 99.50 (99.40–99.59) | 97.89 (97.37–98.35) | 97.99 (97.61–98.32) |
| InceptionV3 | 90.14 (89.76–90.53) | 88.47 (87.35–89.58) | 89.00 (88.23–89.83) |
| ResNet50V2 | 99.49 (99.39–99.58) | 97.32 (96.75–97.85) | 97.37 (96.99–97.75) |
| **Proposed ConvNeXt-GCN** | **99.95 (99.91–99.98)** | **99.15 (98.87–99.39)** | **99.05 (98.81–99.29)** |

**Figure 2. Performance comparison of the proposed ConvNeXt-GCN framework with state-of-the-art deep learning models.**

### Results Discussion

The experimental results demonstrate that the proposed ConvNeXt-GCN framework achieves the highest recognition performance among all evaluated architectures. Specifically, the proposed model obtains 99.95% training accuracy, 99.15% validation accuracy, and 99.05% testing accuracy.

In comparison, DenseNet121, MobileNet, InceptionV3, and ResNet50V2 achieve testing accuracies of 97.22%, 97.99%, 89.00%, and 97.37%, respectively. The proposed framework therefore achieves absolute testing accuracy improvements of 1.83, 1.06, 10.05, and 1.68 percentage points over these respective baseline architectures.

Furthermore, the proposed model maintains consistently high performance across the training, validation, and testing stages. The narrow intervals reported alongside its accuracy values also indicate a relatively stable performance profile under the reported evaluation protocol.

These findings demonstrate the effectiveness of combining ConvNeXt-based hierarchical visual feature extraction with graph-based relational representation learning for recognizing visually diverse freshwater fish species.

## 🔬 Statistical Significance Analysis

To further investigate the reliability of the observed performance improvements, a Wilcoxon signed-rank test was conducted between the proposed ConvNeXt-GCN framework and each competing architecture using 10 paired experimental runs.

The Wilcoxon signed-rank test is a nonparametric statistical method used to examine whether the paired performance differences between two models are statistically significant. It is particularly useful for evaluating model performance differences without requiring the assumption of normally distributed paired observations.

### Wilcoxon Signed-Rank Test Results

| Comparison | W Statistic | p-value | Significance |
|---|---:|---:|---|
| Proposed vs. DenseNet121 | 2 | 0.004 | Significant |
| Proposed vs. MobileNet | 4 | 0.009 | Significant |
| Proposed vs. InceptionV3 | 1 | 0.002 | Significant |
| Proposed vs. ResNet50V2 | 3 | 0.007 | Significant |

**Figure 3. Wilcoxon signed-rank test comparing the proposed ConvNeXt-GCN framework with competing architectures over 10 paired experimental runs.**

### Statistical Analysis and Interpretation

The statistical analysis demonstrates that the proposed ConvNeXt-GCN framework achieves statistically significant performance differences compared with all four baseline architectures. Specifically, the Wilcoxon signed-rank test produces p-values of 0.004, 0.009, 0.002, and 0.007 for comparisons against DenseNet121, MobileNet, InceptionV3, and ResNet50V2, respectively.

All reported p-values are below the conventional significance threshold of 0.05, indicating statistically significant paired differences between the proposed framework and the competing models across the evaluated runs.

These findings provide additional statistical evidence supporting the comparative performance results and suggest that the observed improvements are not simply attributable to random variation across the paired experimental runs.

However, the interpretation of these results should consider the number of paired runs and the statistical testing protocol employed.

## 🛠️ Technologies and Tools

The project is designed around modern deep learning and computer vision technologies.

- Python
- PyTorch
- Torchvision
- ConvNeXt-Tiny
- Graph Neural Networks
- Graph Convolutional Networks
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## 🌍 Potential Applications

The proposed framework has potential applications in several areas:

- Automated freshwater fish identification.
- Fisheries resource management.
- Aquaculture monitoring.
- Freshwater biodiversity documentation.
- Intelligent mobile-based fish recognition.
- Digital fish species information systems.

## 🔬 Research Significance

This research explores the integration of convolutional neural networks and graph-based learning for freshwater fish species recognition. By combining hierarchical visual feature extraction with relational representation learning, the proposed ConvNeXt-GCN framework investigates an alternative approach to conventional image classification.

In addition to introducing a hybrid recognition architecture, this study contributes a collected dataset of 28 freshwater fish species from Bangladesh, which is publicly available through Mendeley Data. The comparative experimental results and statistical significance analysis further provide evidence of the effectiveness of the proposed framework.

Overall, this work contributes to the development of intelligent fish recognition systems and supports future research in freshwater biodiversity monitoring, fisheries management, and computer vision-based aquatic species identification.
