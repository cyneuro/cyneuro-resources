(content:training:software_workflows)=
# Software and workflows

## Software tutorials
- <a href="https://colab.research.google.com/github/cyneuro/CI-BioEng-Class/blob/main/cs4001_terminal.ipynb" target="_blank">The Unix Terminal</a>
- <a href="https://colab.research.google.com/github/cyneuro/CI-BioEng-Class/blob/main/cs4001_git.ipynb" target="_blank">Git & GitHub</a>

## Neuroscience workflows

- <a href="https://colab.research.google.com/github/cyneuro/Basics-of-Neurons-and-Networks/blob/main/B3_MoreProperties/AdditionalProperties.ipynb" target="_blank">Simulating a single cell model with Neuron and plotting the FI curve</a>
- <a href="https://colab.research.google.com/github/cyneuro/CI-BioEng-Class/blob/main/cs4001_allen.ipynb" target="_blank">Downloading and building cells from AllenDB</a>

## Mini-projects

**Mini-project 1: GUI-based quiz system**

Develop an adaptive learning tool for a Math topic (such as solving quadratic equations), or a Python topic (such as list manipulation), or a Physics topic (such as estimating motion of a projectile).

Requirements:

1. The tool should be a Python program and should include a graphical user interface (GUI). The user interacts with the program via UI buttons.

2. The program should have a tiny database of questions from 3 difficulty levels (easy, medium, hard). When the user starts the program, they are presented with questions from the "easy" category. Once the user answers 3 "easy" questions correctly, the program should start showing "medium" questions. After 3 correct responses, the program should switch to the "hard" questions. The database should contain at least 5 questions in each category.

**Mini-project 2: Automated EEG data analysis**

Develop an automated system for EEG data analysis and visualization.

1. Get familiar with what [EEG data are](https://en.wikipedia.org/wiki/Electroencephalography), [electrode positioning systmes](https://en.wikipedia.org/wiki/10–20_system_(EEG)) and the notion of a [montage](https://www.learningeeg.com/montages-and-technical-components). Summarize advantages and disadvantages of EEG recordings and differences between bipolar and referential montages.
2. Find any public EEG dataset (e.g., [EEG Brainwave Dataset: Feeling Emotions](https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions)) and implement the following workflow:
   
   1. The user selects the type of montage (referential or bipolar) and provides two frequency values (low and high).
   
   2. The program re-references the data according to the type of montage and applies a [band-pass filter](https://en.wikipedia.org/wiki/Band-pass_filter) using the provided frequencies.
   
   3. The program plots the voltage trace of each processed channel in a dashboard format (i.e., all channels over a grid) and displays aggregate characteristics of each trace (e.g., mean, variance, Fano factor, etc.)
   
   4. (Optional) The program predicts some target variable using the data and displays prediction results.

You can use [this notebook](https://github.com/cyneuro/neuro_communication/blob/main/eeg_emotion_classification.ipynb) for reference, but you are not required to implement the prediction model.

**Mini-project 3: Atomated workflow for PCM on public fMRI data**

TBD

**Mini-project 4: Classification of accelerometer data using micro:bit**

TBD

**Mini-project 5: Comparison of computational capabilities of micro:bit, PC and FABRIC**

TBD

## Final projects

1. Analysis of substance abuse data.
    
    1.1. PCM using a combination of sMRI and fMRI data.

    1.2. Combining PCM and additional features derived from fMRI data.

    1.3. TBD: projects from collaborators (St. Louis, Rolla, Alabama).

2. Automated workflow for fMRI data processing.
3. Movement prediction using micro:bot.
4. Automated workflow for training a machine learning model with data from online databases.
6. Automated workflow for genetics data classification.