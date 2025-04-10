# Citrus Leaves Dataset

This repository contains the Citrus Leaves dataset, which is a collection of images of healthy and unhealthy citrus leaves. The dataset is sourced from Mendeley Data and is also available through TensorFlow Datasets.

## Description

(1) In agriculture, plant diseases are primarily responsible for the reduction in production which causes economic losses. In plants, citrus is used as a major source of nutrients like vitamin C throughout the world. However, ‘Citrus’ diseases badly effect the production and quality of citrus fruits.

(2) The computer vision and image processing techniques have been widely used for detection and classification of diseases in plants.

(3) The dataset contains an image gallery of healthy and unhealthy citrus fruits and leaves that could be usable for the researchers to prevent plants from diseases using advanced computer vision techniques. The disease targeted in the data sets are the Blackspot, Canker, Scab, Greening, and Melanose.

(4) The dataset contains 759 images of healthy and unhealthy images for both Citrus fruits and leaves collectively. Each image contains 256 * 25 dimensions with 72 dpi resolution.

(5) All images were acquired  from the Sargodha region, a tropical area of Pakistan under the supervision of Dr. Basharat ALi Saleem, Endeavour Executive Fellow Curtin University · Horticulture Research Laboratory  Postharvest Australia · Bentley

(6) All images were annotated manually by the domain expert Dr. Basharat ALi Saleem to represent their every class such as : For Citrus fruits (Black Spot, Canker, Greening, Scab, and healthy  with total number of 150 images ), For  Citrus Leaves (Black Spot, Canker, Greening, Melanose, and healthy with total number of 609 image)

## Dataset Description

The dataset consists of images of citrus leaves with two main categories:
- Healthy leaves
- Unhealthy leaves (diseased)

### Dataset Statistics
- Total number of images: 1,000+
- Image format: JPG
- Image resolution: Various sizes
- Classes: 2 (Healthy, Unhealthy)

## Dataset Structure

```
citrus_leaves/
├── healthy/         # Contains images of healthy citrus leaves
└── unhealthy/       # Contains images of unhealthy/diseased citrus leaves
```

## Data Source

This dataset is sourced from:
- [Mendeley Data](https://data.mendeley.com/datasets/3f83gxmv57/2)
- [TensorFlow Datasets Catalog](https://www.tensorflow.org/datasets/catalog/citrus_leaves)

## Usage

### Using with TensorFlow

```python
import tensorflow_datasets as tfds

# Load the dataset
dataset = tfds.load('citrus_leaves', split='train')

# Iterate over the dataset
for example in dataset:
    image = example['image']
    label = example['label']
    # Process your data here
```

### Manual Usage

You can also use the dataset manually by accessing the image files directly from the directory structure.

## Citation

If you use this dataset in your research, please cite:

```
@article{rauf2019citrus,
  title={A citrus fruits and leaves dataset for detection and classification of
citrus diseases through machine learning},
  author={Rauf, Hafiz Tayyab and Saleem, Basharat Ali and Lali, M Ikram Ullah
and Khan, Muhammad Attique and Sharif, Muhammad and Bukhari, Syed Ahmad Chan},
  journal={Data in brief},
  volume={26},
  pages={104340},
  year={2019},
  publisher={Elsevier}
}
```

## Acknowledgments

- Original dataset creators: Kumar, Rajesh et al.
- Mendeley Data for hosting the dataset
- TensorFlow Datasets team for making the dataset easily accessible

## Contact

For any questions or issues regarding this dataset, please open an issue in this repository.

## License

This dataset is available under the CC BY 4.0 license. See the original sources for more details.
