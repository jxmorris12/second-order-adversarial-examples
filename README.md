This repository contains code and datasets for the experiments in the paper "Second-order adversarial examples" submitted to the [BlackboxNLP workshop](https://blackboxnlp.github.io/cfp.html) at EMNLP 2020. All experiments were run in Google Colab using a single Tesla K80 GPU. `figs/` contains figures shown in the paper. All experiments were implemented in the following Jupyter notebooks:

- `s3_constraint_robustness_curve_demo.ipynb` contains code for generating the sample Constraint Robustness Curve in (Figure 2)
- Each adversarial attack (both first and second-order) was implemented in one Jupyter notebook per dataset. These notebooks contain the same code, just a different dataset + victim models, and different attack outputs.
	- `s5_attack_sst2.ipynb`: SST-2 sentiment classification dataset
	- `s5_attack_snli.ipynb`: SNLI entailment dataset
	- `s5_attack_mr.ipynb`: Rotten Tomatoes/Movie Review/MR sentiment classification dataset


