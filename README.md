# Learning Hamiltonians of constrained mechanical systems

This repository collects the Notebooks written for the numerical experiments of the paper: https://arxiv.org/abs/2201.13254

The Notebooks are divided into codes for Constrained and Unconstrained systems.



#### Experiment with physically informed regularization

In the notebook NoisyTrajectoriesRegularized.ipynb we work with the Hamiltonian system having Hamiltonian
$$
H\left(q_{1}, q_{2}, p_{1}, p_{2}\right)=\frac{q_{1}^{2}+p_{1}^{2}}{2}+\frac{p_{2}^{2}}{2}+\frac{1}{2} q_{2}^{2}+\frac{1}{4} q_{2}^{4}=h_{1}\left(q_{1}, p_{1}\right)+h_{2}\left(q_{2}, p_{2}\right).
$$
Here we test if training adding a regularization term of the form
$$
\mu \sum_{i \in \mathcal{I}}\left |G\left(\hat{y}_{k}^{i}\right)-G\left(x_{k}\right)\right|
$$
to the loss function, with $G(q_1,q_2,p_1,p_2)=h_1(q_1,p_1)$ allows to get better results for training sets with noisy trajectories.

