# *F*ields of *T*he *W*orld (FTW)

## About 
*F*ields of *T*he *W*orld (FTW) is an open, community-driven initiative to advance global agricultural intelligence by building and sharing tools, datasets, and models for field boundary detection. Originally launched as a benchmark dataset, FTW has expanded into a full ecosystem supporting research, development, and deployment of geospatial workflows for the cloud.

We aim to make field-scale analysis more accessible, reproducible, and comparable, enabling better land use monitoring, food security efforts, and agricultural insights. You can learn more at [fieldsofthe.world](https://fieldsofthe.world).

This GitHub organization contains all the code to download and use the FTW Dataset, along with other related repositories.

The dataset is available on Source Cooperative ([link](https://beta.source.coop/kerner-lab/fields-of-the-world/)), and the [ftw-baselines](https://github.com/fieldsoftheworld/ftw-baselines) 
repository provides tools to easily get the data and start building models. You can also suggest new datasets to add in the [ftw-datasets-list issue tracker](https://github.com/fieldsoftheworld/ftw-datasets-list/issues)

---

## 🔎 What's in the FTW Ecosystem?

### 🗂️ FTW Benchmark Dataset  
Originally the core of the initiative, the **FTW Benchmark Dataset** is a global collection of labeled agricultural field boundaries, designed to benchmark model performance and support open research. It aggregates and harmonizes a number of open datasets into 1.6 million parcel boundaries and over 70,000 samples covering diverse agricultural landscapes across 4 continents and 24 countries.

**What’s included in the Benchmark Dataset?**  
- Publicly available, labeled field boundaries from around the world  
- Uniform data formatting and metadata schema  
- A maintained subset of training/validation/test data  
- Tools to evaluate model performance on shared benchmarks  
- Contribution guidelines for submitting new datasets


### 🧠 FTW Baseline Models  
Reference implementations of machine learning models trained on the FTW Benchmark Dataset. These models offer starting points and performance baselines for researchers and practitioners.

### 🛠️ FTW Tools  
A growing suite of tools to support end-to-end workflows:
- **Data access tools**: Python libraries and CLI tools to download and work with the benchmark dataset  
- **Inference tools**: Scripts and utilities to run field boundary detection on new imagery  
- **Formatting tools**: Resources to convert raw data into FTW-compliant format (e.g., fiboa to FTW train/test split)  
- **QGIS Plugin**: A plugin to browse and interact with field data within QGIS

### 🌐 FTW Web App  
A browser-based interface to explore, select, and analyze scenes using FTW models and data. 

### 📡 FTW Source Data  
Curated public datasets of manually labeled field boundaries—such as those hosted on [fiboa.org](https://fiboa.org)—that may serve as inputs to the benchmark dataset. These are raw sources prior to FTW formatting.

### 🗺️ FTW Data Products  
Large-scale outputs of model-inferred field boundaries (e.g., country-wide field maps). These are versioned and published for external research, planning, and applications.

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
