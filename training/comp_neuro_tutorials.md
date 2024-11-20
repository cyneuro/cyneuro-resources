(content:training:comp_neuro_tutorials)=
# Computational Neuroscience Tutorials

- All tutorials can be run either on a local computer or in Google Colab. 
- To run in Colab there is no need to download the repo – instead, click on the folder and then the .ipynb file. There will be a button at the start of the notebook which says 'Open in Colab'. Click this button, and the notebook will be loaded into Colab. 
- If running on a local machine, make sure that Jupyter is installed with the Python packages `neuron` and `ipywidgets`.

## Tutorials

<!--- ## - <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/B1_BasicsSingleNeuron" target="_blank">B1-CreatingSingleCell</a>
- <a href="https://colab.research.google.com/github/cyneuro/Basics-of-Neurons-and-Networks/blob/main/B1_BasicsSingleNeuron/B1_SingleNeuronBio&Model.ipynb" target="_blank">B1-CreatingSingleCell</a>  
     Goes over the components of a neuron (in particular the soma) and asks the students to make the biological model and electrical circuit. It then goes over how the soma is simulated in NEURON and the default values for properties of the section created. It then goes over inserting the passive and active channels and how to voltage/current clamp for a simulation. Lastly, an interactive simulation is given to show exactly how the soma looks with the bilayer, the fact that it is polarized, and that channels are actually inserted into the soma.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/B2_NeuronProperties" target="_blank">B2-CableTheory</a>
  
    Goes over how to create a dendrite and what electrotonic distance is and how length constant is a part of it. Then it goes over how it is still transient by showing the voltage change in specific segments through the simulation. It then goes over how to calculate the length constant and why it is important.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/B3_MoreProperties" target="_blank">B3-Propagation</a>
  
    Goes over what input resistance, the fact that it is a constant, and how to calculate it and asks some questions. It then goes over what the FI curve is and plots it for the given cell from the currents -1nA to 2nA. Lastly, it goes over what Nodes of Ranvier and Myelin sheaths are and how they contribute to AP propagation down an axon by adding them on to the axon. It also asks how certain factors affect the propagation speed.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/S1_PassiveMembrane" target="_blank">S1-PassiveMembrane</a>
  
    A simple notebook going over NEURON basics and contains a Hodgkin–Huxley model with widgets.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/S2_ActionPotential" target="_blank">S2-ActionPotenial</a>
  
    An educational notebook going over the fundamentals of how a neuron fires and the voltage gated channels responible for the firing. Contains a NEURON model of a soma with widgets.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/S3_Burster" target="_blank">S3-Burster</a>
  
    An educational notebook discussing one way neurons can display a bursting effect. Contains a NEURON model of a soma and axon with widgets.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/S4_Synapses" target="_blank">S4-Synapses</a>
  
    An educational notebook with NEURON model about how synapses operate.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/S5_CPG" target="_blank">S5-CPG</a>
  
    An educational notebook with a NEURON modle about central pattern generates and how differnt movement patterns in horese may arise.

- <a href="https://github.com/cyneuro/Basics-of-Neurons-and-Networks/tree/main/S6_STM_WTA" target="_blank">S6-STM-WTA Networks</a>
  
    Educational notebooks talking about short term memory(STM) and winner take all(WTA) networks


