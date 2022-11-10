---
layout: default
---
# Analysing the Robustness of Controllers for Information Transfer in Quantum Spin-1/2 Networks
> This is the work I completed as a part of my Summer Research Internship in Quantum Control at Cardiff University. The project was supervised by Dr Frank C Langbein.
View on [GitHub](https://github.com/jayantmisra/analysing-robustness-of-controls).

## Abstract

Download [Abstract](assets/abstract-pdf.pdf).


## Poster
![Poster](assets/poster-png.png)
Download [Poster](assets/poster-pdf.pdf).


## Contents of the Poster

### Background
Quantum technologies have very promising applications in networking, simulation, sensing and computing. However, decoherence, arising from unwanted interactions of a device with environment, and fabrication and control signal uncertainties present a particular challenge for Noisy Intermediate Scale Quantum devices. There are two popular ways to mitigate noise and errors and achieve fault tolerance: Error correction/mitigation algorithms and Robust Quantum Control solutions. Error Correction algorithms and Quantum Control solutions are two complementary approaches used to tackle the problem of noise in Quantum technologies.

Quantum Control deals with the study of how the classical world interacts with quantum systems and optimization of these quantum systems to enable useful performance in information processing, sensing and metrology. In this project we work on analysing robust quantum controllers for information transfer in quantum spin-1/2 networks.

### Aim
The aim of this project is to investigate the robustness of the controls schemes achieved from previous gradient-based optimization experiments computationally by calculating the log-sensitivity of the controllers w.r.t. structured perturbations: delta*S, with structure S and the strength of the perturbation ‘delta’.

### Methodology
- First, we calculated the transfer fidelity error (or infidelity) and the log-sensitivity of the top 100 controllers obtained from previous optimization experiments. A dataset of 1000 controllers found via gradient-based optimal quantum control for information transfer in spin-1/2 XX rings was used [1].
- To further analyse the quality and robustness of the controllers, we took the average fidelity error and average log-sensitivity across 1000 randomly structured perturbations. And also calculated the Spearman correlation coefficient for the average fidelity error and the average log-sensitivity to assess their statistical dependence.
- For the next part, we analysed the structure of the spin rings by calculating the log-sensitivity of the fidelity curve for each spin and coupling individually w.r.t. structured perturbation for delta(0 - 0.1).

### Results

#### More Results [Not Included in the Poster]

### Conclusion
- The Spearman Correlation coefficient for our data ranges from 0.26 to 0.87 which demonstrates that there is some statistical dependence between transfer fidelity and log-sensitivity. 
- We know that very high fidelity controllers are also very sensitive, but if the fidelity of the controllers is a bit lower, they are not very sensitive anymore.
- The couplings which are involved in the transfer of information are highly sensitive to noise.
- There are also some cases where the couplings opposite to the couplings which are involved in transfer have high log-sensitivity. 

### References
> [1] FC Langbein, SG Schirmer, EA Jonckheere. Energy Landscape Control Robustness Dataset. (In preparation). 
> [2] F. C. Langbein, S. Schirmer and E. Jonckheere, "Time optimal information transfer in spintronics networks," 2015 54th IEEE Conference on Decision and Control (CDC), 2015, pp. 6454-6459, doi: 10.1109/CDC.2015.7403236.
> [3] Shermer, Sophie & Jonckheere, Edmond & O'Neil, Sean & Langbein, Frank. (2018). Robustness of energy landscape control for spin networks under decoherence.
> [4] Khalid, Irtaza and Weidner, Carrie A. and Jonckheere, Edmond A. and Shermer, Sophie G. and Langbein, Frank C. “Statistically Characterising Robustness and Fidelity of Quantum Controls and Quantum Control Algorithms”. https://arxiv.org/abs/2207.07801
