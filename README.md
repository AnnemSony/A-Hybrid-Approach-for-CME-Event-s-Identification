# A Hybrid Approach for CME Event’s Identification

## Abstract

Halo Coronal Mass Ejections (CMEs) are significant solar events capable of triggering geomagnetic storms that affect space-borne and ground-based systems. Accurate and timely detection of such events is essential for effective space weather forecasting. In this study, we present a hybrid detection framework for halo CMEs using particle data from the SWIS-ASPEX payload onboard India’s Aditya-L1 mission.

Our approach derives physics-informed features from raw solar wind parameters—including flux spike scores, speed jumps, density dips, and thermal shocks—based on solar energetic particle theory. These derived parameters are used as input to three independent detection mechanisms:  
1. **Statistical thresholds:** z-scores, percentiles  
2. **Physics-based rules:** from heliophysics literature  
3. **Unsupervised machine learning:** Isolation Forest model  

A composite decision strategy is employed to identify CME intervals by combining outputs from all three detection layers. The hybrid system reduces false positives while improving detection accuracy, without requiring any labeled training data. Experimental results demonstrate that the ensemble framework reliably identifies CME signatures in complex solar wind environments and shows improved performance over single-method approaches.

This work highlights the potential of integrating domain knowledge with data-driven algorithms to enhance heliophysical event detection and lays a foundation for near-real-time application in future missions.

## Plain Language Summary

We aim to detect halo CME events using data from India Aditya-L1 mission. Our model combines physics thresholds and AI to improve space weather forecasting.

## Introduction

Coronal Mass Ejections (CMEs) are among the most powerful eruptive events in the heliosphere, involving the sudden expulsion of large volumes of magnetized plasma from the solar corona into interplanetary space. A single CME can release up to 10¹² kg of plasma and energy equivalent to billions of nuclear bombs, propagating through the solar wind and interacting with planetary magnetospheres. These events are primarily triggered by magnetic reconnection and destabilization.




## Requirements

- Python 3.9
- Jupyter Notebook
- scikit-learn

## Usage

1. **Clone the repository**  
   ```bash
   git clone https://github.com/AnnemSony/A-Hybrid-Approach-for-CME-Event-s-Identification.git
