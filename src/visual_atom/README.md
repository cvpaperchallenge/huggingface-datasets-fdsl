---
language: en
license: mit
tags:
- fdsl
annotations_creators: formula-generated
pretty_name: VisualAtom
size_categories: 1M<n<10M
source_datasets: original
task_categories: image-classification
---

# Dataset Card for VisualAtom

## Table of Contents

- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks](#supported-tasks-and-leaderboards)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-fields)
  - [Data Splits](#data-splits)
- [Dataset Creation](#dataset-creation)
  - [Curation Rationale](#curation-rationale)
  - [Source Data](#source-data)
  - [Annotations](#annotations)
  - [Personal and Sensitive Information](#personal-and-sensitive-information)
- [Considerations for Using the Data](#considerations-for-using-the-data)
  - [Social Impact of Dataset](#social-impact-of-dataset)
  - [Discussion of Biases](#discussion-of-biases)
  - [Other Known Limitations](#other-known-limitations)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)
  - [Contributions](#contributions)

## Dataset Description

- **Homepage:** https://masora1030.github.io/Visual-Atoms-Pre-training-Vision-Transformers-with-Sinusoidal-Waves/
- **Repository:** https://github.com/masora1030/CVPR2023-FDSL-on-VisualAtom
- **Paper:** https://arxiv.org/abs/2303.01112
- **Leaderboard:** NA
- **Point of Contact:** Sora Takashima: soraemonpockt@gmail.com

### Dataset Summary

VisualAtom is an image dataset desigened for Formula-Driven Supervised Learning (FDSL), where every data point is automatically generated and labeled through mathematical formulas. Drawing inspiration from Bohr’s atomic model, it employs circular harmonics as its mathematical basis. This unique approach allows VisualAtom to generate contour-oriented images more systematically and effectively than existing FDSL datasets.

💡 Note that the VisualAtom dataset available here is identical to the one used in the evaluations presented in the paper, referred to as VisualAtom-1k. With the [official code](https://github.com/masora1030/CVPR2023-FDSL-on-VisualAtom), you can easily create a custom VisualAtom dataset, allowing for any specific classes and instance counts to suit your particular requirements.

### Supported Tasks and Leaderboards

- `image-classification`: The goal of this task is to classify a given image into one of 1000 classes. An official leaderboard is not provided for this dataset.

### Languages

All data in this dataset are automatically generated and labeled based on mathematical formulas, so they are not represented in any specific natural language. The class labels directly use the numerical values of the parameters inputted into the formulas.

## Dataset Structure

### Data Instances

TBD

### Data Fields

TBD

### Data Splits

TBD

|             |train  |validation| test  |
|-------------|------:|---------:|------:|
|# of images  | TBD   |0         |0      |


## Dataset Creation

### Curation Rationale

Formula-Driven Supervised Learning (FDSL) datasets, including VisualAtom, are introduced to address key limitations often encountered with real-image datasets like ImageNet, including (i) data ownership and licensing restrictions, (ii) high costs associated with manual annotation, (iii) the presence of social and ethical biases, and (iv) restricted access to large-scale datasets, such as JFT-300M. FDSL addresses these challenges by utilizing formula-based, automatically generated images and labels, facilitating model pre-training entirely independent of natural image data. This approach offers a scalable, unbiased, and legally unencumbered alternative to traditional real-image datasets.

### Source Data

#### Initial Data Collection and Normalization

All data in this dataset is generated and labeled entirely through automated processes based on mathematical formulas.

#### Who are the source language producers?

All data and labels in this dataset are fully generated through automated processes based on mathematical formulas, with no reliance on external data sources or platforms.

### Annotations

#### Annotation process

Class labels are automatically assigned as annotations, directly reflecting the numerical values of the parameters used in data generation.

#### Who are the annotators?

As the process is fully automated, no human annotators are involved at any stage.

### Personal and Sensitive Information

All data is generated automatically through mathematical formulas, ensuring that no personal or sensitive information is included.

## Considerations for Using the Data

### Social Impact of Dataset

The FDSL dataset category, including VisualAtom, marks an important new paradigm designed to address key challenges associated with real-image datasets, as detailed in the "Curation Rationale" section. Additionally, VisualAtom’s generating formulas have been carefully crafted based on in-depth analyses of existing FDSL datasets, establishing it as a foundational benchmark for advancing future FDSL research.

### Discussion of Biases

- All data in this dataset are automatically generated and labeled based on mathematical formulas, making it free from social or ethical biases.
- A [study](https://arxiv.org/abs/1811.12231) has reported that models pre-trained on ImageNet exhibit a texture bias, whereas models trained on VisualAtom have been empirically found to acquire a bias more oriented toward shape.

### Other Known Limitations

TBD

## Additional Information

### Dataset Curators

All data in this dataset is automatically generated and labeled based on mathematical formulas, eliminating the need for any human curators.

### Licensing Information

This dataset is licensed under the MIT License.

### Citation Information

```bibtex
@inproceedings{takashima2023visual,
  title={Visual atoms: Pre-training vision transformers with sinusoidal waves},
  author={Takashima, Sora and Hayamizu, Ryo and Inoue, Nakamasa and Kataoka, Hirokatsu and Yokota, Rio},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={18579--18588},
  year={2023}
}
```

### Contributions

Thanks to following contributors for adding this dataset:
- [@gatheluck](https://github.com/gatheluck)