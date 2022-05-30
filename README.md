# Learning Hamiltonians of constrained mechanical systems

This repository collects the Notebooks written for the numerical experiments of the paper: [Arxiv Preprint](https://arxiv.org/abs/2201.13254)

The paper has been presented in a seminar here : [Seminar](http://y2u.be/tAIGUkXp-Ck)

The Notebooks are divided into codes for Constrained and Unconstrained systems.

#### Experiment with unconstrained 4-dimensional system

In the notebook Unconstrained_Hamiltonian_R4.ipynb we train a network to approximate a Hamiltonian having kinetic energy that couples the two components of the momentum. 

#### Experiment with physically informed regularization

In the notebook NoisyTrajectoriesRegularized.ipynb we test if training adding a regularization term that promotes the preservation of a known first integral allows to get better results for training sets with noisy trajectories.

#### Experiments with chains of spherical pendula

In the notebook chainOfSphericalPendulums.ipynb we train a network to approximate the dynamcis of a chain of N connected spherical pendula. The number of connected pendula can be changed, and also four numerical integrators that can be adopted in the training are implemented. 

#### Parameter study for spherical pendulum

In the notebook comparisonsParametersSection4.ipynb and the associated collected dataset of experiments CollectedData.csv there are the plots and tables for the parameter study reported in the paper. An alternative way to interact with the dataset is to go at the associated website [Parameter study](https://davidemurari.github.io/learningConstrainedHamiltonians/)
