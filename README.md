## [OffensEval: Identifying and Categorizing Offensive Language in Social Media ](https://competitions.codalab.org/competitions/20011)

This work was done for the SemEval 2019 Task 6: OffenseEval. We participated in two of the three sub-tasks
Sub-task B - Automatic categorization of offense types and Sub-task C - Offense target identification.
Among 75 participating teams in SemEval-2019 sub-task B, our system ranks 6th (with 0.706 macro F1-score). For sub-task C, among the 65 participating teams, our system ranks 9th (with 0.587 macro F1-score).. 

The dataset can be found [here](https://github.com/abishekarun/OffenseEval/blob/master/offenseval-training-v1.tsv) and our paper can be found [here](https://arxiv.org/abs/1906.03692). 

We performed an extensive hyperparameter search across traditional machine learing models for n-gram values and sampling techniques to identify top performing models which we were later used for ensembling to improve performance. We could have performed random search or used package like hyperopt to obtain the best combination but in order to do ensembling later, we chose to do such an extensive explicit optimization. 

|    **Subtask Directory**  | **READme file** |
|--------------------|------------|
| [Subtask-B](https://github.com/abishekarun/OffenseEval/blob/master/subtask_b/) | [1](https://github.com/abishekarun/OffenseEval/blob/master/subtask_b/README.md)|
| [Subtask-C](https://github.com/abishekarun/OffenseEval/blob/master/subtask_c/) | [2](https://github.com/abishekarun/OffenseEval/blob/master/subtask_c/README.md) |

Final submission metrics results can be seen [here](https://nbviewer.jupyter.org/github/abishekarun/OffenseEval/blob/master/results.ipynb)

The resources that helped me are:

+ [Sampling Techniques for Highly Imbalanced Data](https://medium.com/anomaly-detection-with-python-and-r/sampling-techniques-for-extremely-imbalanced-data-part-i-under-sampling-a8dbc3d8d6d8)
+ [Near Miss in python](https://medium.com/@saeedAR/smote-and-near-miss-in-python-machine-learning-in-imbalanced-datasets-b7976d9a7a79)
+ [Comparison of undersampling methods](https://imbalanced-learn.readthedocs.io/en/stable/auto_examples/under-sampling/plot_comparison_under_sampling.html)
+ [Imbalanced Data classification](https://chih-ling-hsu.github.io/2017/07/25/Imbalanced-Data-Classification)
+ [Survey of Resampling Techniques](https://arxiv.org/pdf/1608.06048.pdf)
+ [Guide to ensemble methods](https://towardsdatascience.com/simple-guide-for-ensemble-learning-methods-d87cc68705a2)
+ [Ensemble Learning](https://blog.statsbot.co/ensemble-learning-d1dcd548e936)
+ [Why ensemble](https://towardsdatascience.com/ensemble-methods-in-machine-learning-what-are-they-and-why-use-them-68ec3f9fef5f)