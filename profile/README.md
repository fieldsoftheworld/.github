# *F*ields of *T*he *W*orld (FTW)

## About 
*F*ields of *T*he *W*orld (FTW) is a comprehensive benchmark dataset designed to enhance the development of machine learning models for instance segmentation of agricultural field boundaries. 
This dataset aims to meet the growing need for accurate and scalable field boundary data for global agricultural monitoring and assessments.

This github organization contains all the code to download and use the FTW dataset, along with other related repositories.

The dataset is available on Source Cooperative ([link](https://beta.source.coop/kerner-lab/fields-of-the-world/)), and the [ftw-datasets](https://github.com/fieldsoftheworld/ftw-baselines) 
repository provides tools to easily get the data and start building models.

### Key Features:

1. **Near-Global Coverage**: FTW spans four continents—Europe, Africa, Asia, and South America—covering diverse agricultural landscapes across 24 countries. This extensive geographic coverage allows for the development of models that can generalize well to different agricultural practices and field types.

2. **Large-Scale Dataset**: With approximately 1.6 million parcel boundaries and over 70,000 samples, FTW is significantly larger than previously available datasets. Each sample includes instance and semantic segmentation masks paired with multi-date, multi-spectral Sentinel-2 satellite images, enabling detailed temporal and spectral analysis.

3. **Multi-class Segmentation**: The dataset provides masks for both instance segmentation and semantic segmentation with different classes, including:
   - **Instance Segmentation Masks**: To identify individual fields.
   - **Semantic Segmentation Masks**: 
     - Two-class masks: Background and polygon (field).
     - Three-class masks: Background, polygon (field), and boundaries.

4. **Spectral Richness**: The dataset includes RGB (Red, Green, Blue) and NIR (Near-Infrared) spectral bands from Sentinel-2 images.

5. **Temporal Richness**: The dataset includes multi-date imagery to capture different stages of the growing season. Two images with distinct contrast differences were selected to represent these stages. To determine the date ranges for these images, the USDA Crop Calendar was initially referenced and then refined by selecting periods with minimal cloud cover and optimal contrast between the two images.

6. **Comprehensive Data Splits**: The dataset is carefully divided into training, validation, and test sets to ensure accurate evaluation of model performance. For each country, larger tiles are divided into smaller chips measuring 1536x1536 m². To prevent data leakage due to spatial autocorrelation, a blocked random splitting strategy is used. Chips are grouped into 3×3 blocks, with 80% allocated to training, 10% to validation, and 10% to testing.

7. **Metadata and Documentation**: The metadata and documentation provide crucial information to help users effectively interpret and utilize the dataset. It includes key details about the country of focus, temporal data collection windows, grid structures, and the year of collection.

   1. **Country**: The geographic region the dataset focuses on.
   2. **Crop Types**: Crop types used to filter the polygons in the dataset, with specific keywords used for filtering.
   3. **Seasons**: Date ranges defining the temporal windows for data collection.
   4. **Year of Collection**: The year when the polygon boundaries were captured.
   5. **Grids**: Larger grids from which smaller chips are derived, with some grids spatially separated to optimize area coverage.
