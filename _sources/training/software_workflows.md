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
2. Find **any** public EEG dataset (e.g., [Emotion Recognition using EEG and Computer Games](https://www.kaggle.com/datasets/wajahat1064/emotion-recognition-using-eeg-and-computer-games/data), [EEG Brainwave Dataset: Feeling Emotions](https://www.kaggle.com/datasets/birdy654/eeg-brainwave-dataset-feeling-emotions)) and implement the following workflow:
   
   1. The user selects the type of montage (referential or bipolar) and provides two frequency values (low and high).
   
   2. The program re-references the data according to the type of montage and applies a [band-pass filter](https://en.wikipedia.org/wiki/Band-pass_filter) using the provided frequencies.
   
   3. The program plots the voltage trace of each processed channel in a dashboard format (i.e., all channels over a grid) and displays aggregate characteristics of each trace (e.g., mean, variance, Fano factor, etc.)
   
   4. (Optional) The program predicts some target variable using the data and displays prediction results.

You can use [this notebook](https://github.com/cyneuro/neuro_communication/blob/main/eeg_emotion_classification.ipynb), which explores the Computer Games dataset from above, for reference, but you are not required to implement the prediction model. 

**Note:** public EEG datasets can lack descriptions and can be tricky to process – you might need to mine the dataset's description to understand which column corresponds to which electrode, etc. However, if you find that a dataset misses crucial information, it might be wiser to switch to a different dataset early.

**Mini-project 3: Classification of accelerometer data using the micro:bit**

Develop a workflow for classifying accelerometer data recorded with the micro:bit.

1. Study the [Movement data logger](https://microbit.org/projects/make-it-code-it/movement-data-logger/) tutorial to learn about accelerometer data recording with micro:bit. These additional tutorials might be useful: [Python data logger](https://microbit.org/projects/make-it-code-it/python-wireless-data-logger/), [Sensitive step counter](https://microbit.org/projects/make-it-code-it/sensitive-step-counter/?editor=python), [User guide – Data logging](https://microbit.org/get-started/user-guide/data-logging/#what-is-data-logging?).

2. Create a MakeCode or Python script to record accelerometer data from the micro:bit to your PC. You can transfer the data either via a wire or through a radio connection.

3. Record the following movement sequence: 
   - Hold the micro:bit steady for 5 seconds,
   - Shake the micro:bit for 5 seconds,
   - Hold the micro:bit steady for 5 seconds,
   - Shake the micro:bit for 5 seconds.

You should get approximately 20 seconds of recorded data.

4. Use [this notebook](https://colab.research.google.com/github/cyneuro/ML_camp/blob/main/camp_logreg_microbit.ipynb) to estimate a model for classifying whether the micro:bit is being held steady or being shaken. The notebook uses logistic regression as an example, but you are free to use any other model or create a rule-based classification system. Report the classification accuracy and give suggestions on how to improve it.

**Mini-project 4: Comparison of computational capabilities of the micro:bit, PC and FABRIC**

Compare computational capabilities of devices across 3 tiers: microprocessor (using the micro:bit), PC (using your laptop), cluster (using FABRIC).

1. Choose a difficult computational problem, e.g., calculating a factorial of a large number, inverting a large matrix, constructing a long series of prime numbers, sorting a large array, searching for patterns in a large text, etc.
2. Implement scripts which demonstrate a solution to this problem using both serial and parallel programming.
3. Run your scripts on the micro:bit, your PC and FABRIC and measure the run time. Make a plot which demonstrates gains and losses in simulation time.
4. (Optional) Record and present other efficiency metrics such as RAM usage, network usage, etc.

## Final projects

Below is a list of topics for the final projects. Each topic is followed by general guidelines; however, you are free to choose a particular implementation. You can also suggest your own project topic as long as it is related to neuroscience and/or neural engineering.

1. Analysis of neural data.
    
   1.1. **PCM using sMRI data, fMRI data or a combination of both.**

   Predictive connectome analysis (PCM) is a popular technique for analyzing brain connectivity. Traditionally, connectome matrices were built based on functional imaging data; however, [a recent study](https://www.frontiersin.org/journals/neuroscience/articles/10.3389/fnins.2021.629478/full) showed that combining functional and structural features might give better insights into brain organization. Find an sMRI/fMRI/sMRI+fMRI dataset and identify features which might help predict connectivity between brain regions.

   1.2. TBD: projects from collaborators (Rolla, Alabama).

   1.3 **Automated workflow for sMRI/fMRI data processing.**

   sMRI/fMRI processing involves several important steps such as movement correction and parcellation. Luckily, these steps are implemented in [FreeSurfer](https://freesurfer.net). Implement a worflow for a particular problem that uses FreeSurfer to process user-provided sMRI/fMRI data. As an example, the following materials cover analysis of resting-state fMRI data: [slides](https://mailmissouri-my.sharepoint.com/:b:/g/personal/nairs_umsystem_edu/EQIZ4jjrW81FhJrLcFsoebgB25-teaHs7clIQDeFkwVdQA?e=3yF4tG), [video](https://mailmissouri-my.sharepoint.com/:v:/g/personal/nairs_umsystem_edu/EXWeW3rWRR1AqlPKiLfBuMsBqjJEDdTnOvFm9bB-mUJp1A?e=M9n5ew).

   1.4 **Automated workflow for DSP of medical datasets.**

   Medical data come in a variety of spatial and temporal resolutions, ranging from the whole-brain recordings (EEG) to recordings from individual cells (single unit data). Choose a medical dataset and implement a workflow for performing digital signal processing (DSP) and analysis of the results. 

2. **Movement prediction using micro:bot.**

   The [micro:bot](https://www.eaieducation.com/microbot-eai-352254.html?srsltid=AfmBOor5ZghgKP7l1nNjO9IvvEwx0jeq66K8iGxbp82ljKsNhSyq0rK2) is a small programmable robot operated by the micro:bit. Implement a workflow for interactive movement control that reads data from the micro:bot's camera and uses a predictive model run on a micro:bit to determine the robot's next movemement. 

3. **Automated workflow for training a machine learning model with data from online databases.**

   Neural databases (e.g., [AllenDB](https://celltypes.brain-map.org), [DANDI](https://dandiarchive.org)) are becoming increasingly popular. Implement a workflow runnable on FABRIC or CloudLab that efficiently retrieves data from one of these databases and uses it for training of a machine learning model.


4. **Automated workflow for genetics data classification.**

   4.1 **Implement DNA-seq genome variant calling (.fastq to .vcf) followed phylogeny analysis**

   Use the dataset available for DNA-seq at [link](https://github.com/raopr/AVAH/blob/master/misc/sampleURLs-vlarge.txt). For more information on this, please refer to Module 11 Lecture ppt, where guided information with hands-on tutorial is mentioned.

   4.2 **Implement RNA-seq genome variant calling (.fastq to .vcf) followed phylogeny analysis**

   Use the dataset available for DNA-seq at [link](https://ieee-dataport.org/open-access/variant-analysis-human-genome-sequences-covid-19-research). For more information on this, please refer to Module 11 Lecture ppt, where guided information with hands-on tutorial is mentioned.

   4.3 **Perform phylogeny analysis on TCGA cancer dataset using  genome variant calling (.fastq to .vcf) workflow**

   Explore and find the .fastq format data at [link](https://portal.gdc.cancer.gov/) and perform the same genetic workflow showed in Module 11 guided project then plot phylogeny tree.

   4.4 **Perform phylogeny analysis on your own explored data using  genome variant calling (.fastq to .vcf) workflow**

   Explore and find the .fastq format data at [link](https://www.internationalgenome.org/data/).