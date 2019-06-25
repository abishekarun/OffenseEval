## [OffensEval: Identifying and Categorizing Offensive Language in Social Media ](https://competitions.codalab.org/competitions/20011)

This work was done for the SemEval 2019 Task 6: OffenseEval Sub-task B - Automatic categorization of offense types. Among 75 participating teams in SemEval-2019 sub-task B, our system ranks 6th (with 0.706 macro F1-score).

The dataset can be found [here](https://github.com/abishekarun/OffenseEval/blob/master/offenseval-training-v1.tsv) and our paper can be found [here](https://arxiv.org/abs/1906.03692). 

We develop baseline models for various combinations of sampling techniques and ngram values. 
We also perform synthetic data generation using nearest neighbours to obtain a balanced dataset and run the same models on this new dataset. Finally, we do ensembling of our best models. 

|    **Model **  | **Jupyter Notebook** |
|--------------------|------------|
| Baseline | [1](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_b/baseline.ipynb)|
| Baseline on New Dataset| [2](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_b/new_data/new_data_baseline.ipynb) |


The resources that helped me are:

+ [Sampling Techniques for Highly Imbalanced Data](https://medium.com/anomaly-detection-with-python-and-r/sampling-techniques-for-extremely-imbalanced-data-part-i-under-sampling-a8dbc3d8d6d8)
+ [Near Miss in python](https://medium.com/@saeedAR/smote-and-near-miss-in-python-machine-learning-in-imbalanced-datasets-b7976d9a7a79)
+ [Why ensemble](https://towardsdatascience.com/ensemble-methods-in-machine-learning-what-are-they-and-why-use-them-68ec3f9fef5f)
+ [Comparison of undersampling methods](https://imbalanced-learn.readthedocs.io/en/stable/auto_examples/under-sampling/plot_comparison_under_sampling.html)
