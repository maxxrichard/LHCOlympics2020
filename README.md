# LHC Olympics 2020
This repository contains the code for the implementation of the problems presented in the challenge. (https://lhco2020.github.io/homepage/)
#### ___Authors___:
* Dr. Rui Zhang
* Maxx Richard Rahman

# Problem
Our goal is to ensure that the LHC search program is sufficiently well-rounded to capture "all" rare and complex signals.  The final state for this Olympics will be more focused (generic multijet events) but the observable phase space and potential BSM parameter space(s) are large: all hadrons in the event can be used for learning (be it "cuts", supervised machine learning, or unsupervised machine learning).

What should be reported:

1. A p-value associated with the dataset having no new particles (null hypothesis).

2. As complete a description of the new physics as possible. For example: the masses and decay modes of all new particles (and uncertainties on those parameters).

3. How many signal events (+uncertainty) are in the dataset (before any selection criteria).

# Dataset
Two types of files (from this Zenodo [link](https://doi.org/10.5281/zenodo.3547721)):

- "Monte Carlo Simulation Background": This is a simulated sample that does not have signal. Be warned that both the physics and the detector modeling for this simulation may not exactly reflect the “Data”.

- "Data": These are the LHCO 2020 black boxes. These samples may contain some new signal(s). We will release three black boxes during this challenge.  The first one was released on November 19. The second one was released on December 4. 

Both the "Simulation" and "Data" have the following event selection: at least one anti-kT R = 1.0 jet with pseudorapidity \|η\| < 2.5 and transverse momentum pT > 1.2 TeV.   For each event, we provide a list of all hadrons (pT, η, φ, pT, η, φ, ...) zero-padded up to 700 hadrons.

# Implementation