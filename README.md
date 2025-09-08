# 📊 Mastering Big Data Handling

This project provides a hands-on analysis of strategies for efficiently processing large datasets that exceed typical memory limits. Using a **2.57 GB dataset** on school donations, this work explores and benchmarks various data handling techniques in Python, comparing their performance in terms of **execution time** and **memory usage**.
<br><br>

### ✨ Features
- **Large Dataset Handling**: Implements methods to process a dataset with over 1.1 million records and a size of 2.57 GB.
- **Optimization Strategies**: Applies and evaluates five key strategies for big data processing:
  - Loading a subset of columns.
  - Processing data in chunks.
  - Optimizing data types (e.g., `object` to `category`).
  - Random sampling of the dataset.
  - Parallel processing with Dask.
- **Library Performance Benchmarking**: Compares the performance of **Pandas**, **Polars**, and **Dask** for loading and processing large data.
- **Comparative Analysis**: Provides clear visualizations and metrics to compare the effectiveness of each strategy and library.
<br>

### 🛠️ Technical Overview
- **Language**: Python
- **Environment**: Google Colab
- **Data Manipulation**: Pandas, NumPy
- **Parallel Computing**: Dask
- **High-Performance DataFrames**: Polars
- **Visualization**: Matplotlib, Seaborn
<br>

### 📁 File Structure
- **big_data.ipynb**: The main Google Colab notebook containing all code for data loading, strategy implementation, performance tracking, and analysis.
<br>

### 🚀 Getting Started

1.  **Set Up Environment**:
    Ensure you have an environment to run Jupyter/Colab notebooks. Google Colab is recommended.

2.  **Install Dependencies**:
    Run the following command in a code cell to install the required libraries:
    ```sh
    pip install pandas numpy dask polars matplotlib seaborn
    ```

3.  **Download the Dataset**:
    The notebook requires the `Projects.csv` file from the School Donation Dataset.
    - Download it from https://www.kaggle.com/datasets/perkymaster/school-donations?select=Projects.csv
    - Upload `Projects.csv` to your Google Colab session's root directory or mount your Google Drive and adjust the file path in the notebook.

4.  **Run the Notebook**:
    Open and execute the cells in `big_data.ipynb` to replicate the analysis and view the performance comparisons.
<br>

### 📊 Dataset Information
- **Title:** School Donation Dataset
- **Source:** https://www.kaggle.com/datasets/perkymaster/school-donations?select=Projects.csv
- **Size:** 2.57 GB (`Projects.csv`)
- **Records:** 1,110,017 rows
<br>

### 🔍 Processing Steps
1.  **Dataset Selection**: A dataset larger than 700MB was chosen to simulate a real-world big data scenario.

2.  **Baseline Inspection**: The dataset was first loaded using a standard `pandas.read_csv()` to establish a baseline for performance and memory usage, confirming the challenges of a naive approach.

3.  **Strategy Implementation**: The five big data handling strategies (Load Less Data, Chunking, Type Optimization, Sampling, and Dask) were implemented and their performance was systematically measured.

4.  **Library Comparison**: The core task of loading the dataset was benchmarked across Pandas (baseline), Polars (multi-threaded), and Dask (parallel processing) to compare their raw speed and memory efficiency.

5.  **Analysis and Conclusion**: The results were compiled, visualized, and discussed to determine the best strategy and library for various use cases, from rapid prototyping to high-performance processing.
<br>

### 🔗 Assignment Source
This project was developed as part of the High Performance Data Processing course. The original assignment instructions and source repository with additional documentation can be found here:
- [*Link to Original Project Repo*](https://github.com/kohxuan/HPDP/tree/main/2425/assignment/A2/bdm/KKK)
<br>

### 🤝 Team: KKK
| Name                                                  | Matric No. |
| :-------------------                                  | :--------- |
| [Koh Li Hui](https://github.com/kohlihui)             | A22EC0059  |
| [Koh Su Xuan](https://github.com/kohxuan)             | A22EC0060  |
<br>
