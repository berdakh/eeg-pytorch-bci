# EEG Motor Imagery Analysis with PyTorch and MNE Python

This repository provides a comprehensive pipeline for analyzing motor imagery EEG data using MNE-Python and PyTorch. It includes preprocessing scripts, CNN model training notebooks, and visualization tools, facilitating research and development in EEG-based brain-computer interfaces (BCIs). 

## Features

* **Data Preprocessing**: Utilizes MNE-Python for EEG data loading, filtering, and epoching.
* **Deep Learning Models**: Implements Convolutional Neural Networks (CNNs) for classifying motor imagery tasks.
* **Visualization**: Provides notebooks for visualizing EEG signals and model performance.
* **Dataset Integration**: Supports multiple publicly available EEG datasets via the MOABB framework.([github.com][1])

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/berdakh/eeg-pytorch.git
   cd eeg-pytorch
   ```



2. **Create a virtual environment (optional but recommended)**:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```



3. **Install required packages**:

   ```bash
   pip install mne==0.18.0
   conda install pytorch torchvision cudatoolkit=10.1 -c pytorch
   pip install braindecode
   ```



*Note: Ensure that [MNE-Python](https://mne.tools/stable/index.html) and [PyTorch](https://pytorch.org/) are installed, as they are central to the functionalities provided.*

## Usage

The repository contains multiple scripts and notebooks, each serving specific purposes. Here's a brief overview:

* **Data Preprocessing**:

  * `nu_smrutils.py`: Contains utility functions for EEG data preprocessing using MNE-Python.([github.com][2])

* **Model Training**:

  * `train_CNN_pooled.ipynb`: Jupyter Notebook for training CNN models on pooled EEG data across subjects.
  * `train_CNN_subspe.ipynb`: Jupyter Notebook for training CNN models on subject-specific EEG data.([github.com][1], [github.com][3])

* **Visualization**:

  * `visualization.ipynb`: Jupyter Notebook for visualizing EEG signals and model performance metrics.([github.com][1])

*To execute a notebook:*

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```



2. Open the desired `.ipynb` file and follow the cells sequentially.

## Datasets

The repository integrates several publicly available EEG datasets through the [Mother of All BCI Benchmarks (MOABB)](http://moabb.neurotechx.com/docs/datasets.html) framework:([github.com][1])

* **BNCI2014001**: EEG data from 9 subjects performing four different motor imagery tasks (left hand, right hand, feet, tongue).
* **BNCI2014004**: EEG data from 9 subjects performing left and right hand motor imagery tasks.
* **Weibo2014**: EEG data from 10 subjects performing simple and compound limb motor imagery tasks.
* **PhysionetMI**: EEG data from 109 subjects performing various motor execution and imagery tasks.([github.com][1])

*Note: Please refer to the MOABB website for detailed information and access to these datasets.*

## Contribution

Contributions are welcome! If you have suggestions, bug reports, or enhancements, please open an issue or submit a pull request.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments

This repository was developed by [Berdakh Abibullaev](https://github.com/berdakh), focusing on EEG motor imagery analysis using MNE-Python and PyTorch.

---

*For detailed explanations and methodologies, refer to the Jupyter Notebooks included in the repository.*

If you need further assistance or have specific questions about any script or functionality, feel free to ask!
 
