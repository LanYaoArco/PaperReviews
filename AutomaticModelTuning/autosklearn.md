### Efficient and Robust Automated Machine Learning: Auto-sklearn ([reference]( https://papers.nips.cc/paper/5872-efficient-and-robust-automated-machine-learning.pdf))

- **Finding instantiation of the ML framework**
	- collect **meta-features** for the current dataset and the previous seen dataset
	- statistical meta-featrues: #data points, distribution of features, data skewness ...
	- compare the meta-features (use `L_1` distance) and rank the 'similarity' the dataset with the existing sets
	- determine which algorithm might be the most suitable setting for the current dataset
	- provide general direction, but not fine-grained performance


- **ML framework**
	- search for hyperparameters within a given search space based with Bayesian optimizer

-  **Ensemble construction of model**
	- why: find the optimal setting for individual model is super time-consuming and easy to overfit
	- store models and automatically ensemble them with the weight
	- how to choose the weight: ensemble selection 
