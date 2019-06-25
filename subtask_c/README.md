## [OffensEval: Identifying and Categorizing Offensive Language in Social Media ](https://competitions.codalab.org/competitions/20011)

This work was done for the SemEval 2019 Task 6: OffenseEval Sub-task C - Offense target identification. Among the 65 participating teams in SemEval-2019 sub-task B, our system ranks 9th (with 0.587 macro F1-score). 

The dataset can be found [here](https://github.com/abishekarun/OffenseEval/blob/master/offenseval-training-v1.tsv) and our paper can be found [here](https://arxiv.org/abs/1906.03692). 

We develop baseline models for various combinations of sampling techniques and ngram values. 
We also perform synthetic data generation using nearest neighbours to obtain a overall balanced dataset, two classes balanced datasets and run the same models on these new datasets. Finally, we do ensembling of our best models. 

Balanced Dataset-1 : Synthetic oversampling of GRP and random oversampling of OTH <br />
Balanced Dataset-2 : Synthetic oversampling of OTH and random oversampling of GRP <br />
Balanced Dataset-3 : Synthetic oversampling of OTH and GRP


|    **Model **  | **Jupyter Notebook** |
|--------------------|------------|
| Baseline | [1](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_c/Baselines.ipynb)|
| Baseline on Balanced Dataset-1| [2](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_c/grp_baselines.ipynb) |
| Baseline on Balanced Dataset-2| [3](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_c/oth_baselines.ipynb) |
| Baseline on Balanced Dataset-3| [4](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_c/all_baselines.ipynb) |
| Ensemble| [5](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/subtask_c/ensemble.ipynb) |


The resources that helped me are:

+ [Imbalanced Data classification](https://chih-ling-hsu.github.io/2017/07/25/Imbalanced-Data-Classification)
+ [Survey of Resampling Techniques](https://arxiv.org/pdf/1608.06048.pdf)
+ [Guide to ensemble methods](https://towardsdatascience.com/simple-guide-for-ensemble-learning-methods-d87cc68705a2)
+ [Ensemble Learning](https://blog.statsbot.co/ensemble-learning-d1dcd548e936)
