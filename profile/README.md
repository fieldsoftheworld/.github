# **F**ields of **T**he **W**orld (FTW)

## About




The goal of **F**ields of **T**he **W**orld (FTW) is to build a global field boundary dataset. The effort originally launched as a benchmark dataset, which is still the core of the effort. FTW has expanded into a full ecosystem supporting research, development, and deployment of geospatial workflows for the cloud. The effort is an open, community-driven initiative to advance global agricultural intelligence by building and sharing tools, datasets, and models for field boundary detection. Field boundaries was an obvious first focus area, and perhaps in the future the effort could go beyond boundaries.

Most countries don’t have comprehensive maps of their agricultural fields, and even fewer have up-to-date information on what crops are growing or whether sustainable practices are being used. Our approach to solving this is to leverage Earth observation data and AI to automatically detect field boundaries at scale. By combining open satellite imagery with machine learning, we aim to build a global, open, and regularly updated map of the world’s fields. The intention is that these field boundaries will enable better land use monitoring, food security efforts, and agricultural insights. You can learn more at [fieldsofthe.world](https://fieldsofthe.world).

This GitHub organization contains all the code to download and use the FTW Benchmark Dataset, along with repositories that make it easy to run FTW models and generate field boundaries.

The dataset is available on Source Cooperative ([source.coop/kerner-lab/fields-of-the-world/](https://source.coop/kerner-lab/fields-of-the-world)), and the [ftw-baselines](https://github.com/fieldsoftheworld/ftw-baselines) repository provides tools to easily get the data and start building models. You can also suggest new datasets to add in the [ftw-datasets-list issue tracker](https://github.com/fieldsoftheworld/ftw-datasets-list/issues)

---

## 🔎 What's in the FTW Ecosystem?

### 🗂️ FTW Benchmark Dataset  

Originally the core of the initiative, the **FTW Benchmark Dataset** is a global collection of labeled agricultural field boundaries, designed to benchmark model performance and support open research. It aggregates and harmonizes a number of open datasets into 1.6 million parcel boundaries and over 70,000 samples covering diverse agricultural landscapes across 4 continents and 24 countries. You can explore and download the dataset from Source Cooperative ([source.coop/kerner-lab/fields-of-the-world/](https://source.coop/kerner-lab/fields-of-the-world)).

**What’s included in the Benchmark Dataset?**  

- Publicly available, labeled field boundaries from around the world  
- Uniform data formatting and metadata schema  
- A maintained subset of training/validation/test data  
- Tools to evaluate model performance on shared benchmarks  
- Contribution guidelines for submitting new datasets

### 🧠 FTW Baseline Models  

Reference implementations of machine learning models trained on the FTW Benchmark Dataset. These models offer starting points and performance baselines for researchers and practitioners. Check out the baseline models at [github.com/fieldsoftheworld/ftw-baselines/releases/tag/v1](https://github.com/fieldsoftheworld/ftw-baselines/releases/tag/v1).

### 🛠️ FTW Tools  

A growing suite of tools to support end-to-end workflows:

- **Data access tools**: Python libraries and CLI tools to download and work with the benchmark dataset (FTW CLI, which you can find in the [ftw-baselines](https://github.com/fieldsoftheworld/ftw-baselines) repository)
- **Inference tools**: Scripts and utilities to run field boundary detection on new imagery (FTW CLI, which you can find in the [ftw-baselines](https://github.com/fieldsoftheworld/ftw-baselines) repository)
- **Formatting tools**: Resources to convert raw data into FTW-compliant format (e.g., fiboa to FTW train/test split) (fiboa CLI, which you can find in the [fiboa/cli](https://github.com/fiboa/cli) repository)
- **QGIS Plugin**: A plugin to browse and interact with field data within QGIS. Currently in alpha ([ftw-qgis-plugin](https://github.com/fieldsoftheworld/ftw-qgis-plugin))

### 🌐 FTW Web App  

A browser-based interface to easily run FTW models in any area of the world. Check out the FTW Web App at [fieldsofthe.world/ftw-inference-app/](https://fieldsofthe.world/ftw-inference-app/).

Improvements to the web app are under progress. See the codebase for the app at [github.com/fieldsoftheworld/ftw-inference-app](https://github.com/fieldsoftheworld/ftw-inference-app).

The web app is powered by an API (see [github.com/fieldsoftheworld/ftw-inference-api](https://github.com/fieldsoftheworld/ftw-inference-api)) and deployed to AWS via [github.com/fieldsoftheworld/ftw-api-deployment](https://github.com/fieldsoftheworld/ftw-api-deployment)

### 🗺️ FTW Data Products  

Large-scale outputs of model-inferred field boundaries (e.g., country-wide field maps). These are versioned and published for external research, planning, and applications.

## Related Work

### **Fi**eld **Bo**undaries for **A**griculture (fiboa)

The **Fi**eld **Bo**undaries for **A**griculture (fiboa) project is focused on making field boundary data openly available in a unified format on a global scale.

Curated public datasets of field boundaries from government sources and hand-labeling campaigns, that may serve as inputs to the benchmark dataset. These are converted to the [fiboa](https://fiboa.org) specification. Fiboa data can be found at [https://source.coop/fiboa](https://source.coop/fiboa).

The data found in the Source Cooperative [kerner-lab](https://source.coop/kerner-lab) organization are in the fiboa format.

In the future, FTW datasets may be sourced from the fiboa datasets prior to FTW subsetting and harmonization.

---

## 🤝 Get Involved

We welcome contributions of:

- Field boundary datasets
- Model improvements
- Tool development
- Promotion and educational materials (blog posts, documentation, talks, papers, social media)
- Feedback and ideas

🧑‍💻 Check out our repositories  
📬 [Follow the journey](https://groups.google.com/g/ftw-community) by joining the 'ftw-community' Google Group  
🌐 [Join the working team](https://groups.google.com/g/ftw-team) meetings by joining the 'ftw-team' Google Group
