This repository contains code and datasets for the experiments in the paper "Second-order adversarial examples" submitted to the [BlackboxNLP workshop](https://blackboxnlp.github.io/cfp.html) at EMNLP 2020. All experiments were run in Google Colab using a single Tesla K80 GPU. `figs/` contains figures shown in the paper. All experiments were implemented in the following Jupyter notebooks:

- `s3_constraint_robustness_curve_demo.ipynb` contains code for generating the sample Constraint Robustness Curve in (Figure 2)
- Each adversarial attack (both first and second-order) was implemented in one Jupyter notebook per dataset. These notebooks contain the same code, just a different dataset + victim models, and different attack outputs.
	- `s5_attack_sst2.ipynb`: SST-2 sentiment classification dataset
	- `s5_attack_snli.ipynb`: SNLI entailment dataset
	- `s5_attack_mr.ipynb`: Rotten Tomatoes/Movie Review/MR sentiment classification dataset

The appendix shows the results of some exploratory data analysis, testing BERTScore and USE on QQP, PAWS, and our custom 'Adversarial SNLI' dataset. These experiments were also conducted in one notebook per dataset:
	- `s99_app_s2_constraints_qqp.ipynb`: QQP (Quora Question Pairs) paraphrase identification dataset
	- `s99_app_s2_constraints_paws.ipynb`: PAWS (Paraphrase Adversaries from Word Scrambling) _adversarial_ paraphrase dataset (PAWS is an adversarially-altered version of QQP)
	- `s99_app_s2_testing_constraints_adversarial_snli.ipynb`: Adversarial SNLI (also contains the code for generating Adversarial SNLI from the original SNLI dataset)
