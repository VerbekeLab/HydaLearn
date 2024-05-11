# HydaLearn: Highly Dynamic Task Weighting for Multi-task Learning with Auxiliary Tasks </br><sub><sub>S. Verboven, H. Chaudary, J. Berrevoets, V. Ginis, W. Verbeke [[MLDM 2022]](https://doi.org/10.1007/s10489-022-03695-x)</sub></sub>

Multitask learning (MTL) can improve performance on one task by sharing representations with one or more related auxiliary tasks. Usually, MTL networks are trained on a composite loss function formed by a fixed weighted combination of separate task losses. In practice, however, static loss weights lead to poor results for two reasons. First, the relevance of the auxiliary tasks gradually drifts throughout the learning process. Second, for minibatch-based optimization, the optimal task weights vary significantly from one update to the next depending on the minibatch sample composition. Here, we introduce HydaLearn, an intelligent weighting algorithm that connects the main-task gain to the individual task gradients, to inform dynamic loss weighting at the minibatch level, addressing the two above shortcomings. We demonstrate significant performance increases on synthetic data and two real-world data sets.

## Repository structure
This repository is organised as follows:
```bash
  |- config.json
  |- main.py
```

## Installing
We have provided a `requirements.txt` file:
```bash
pip install -r requirements.txt
```
Please use the above in a newly created virtual environment to avoid clashing dependencies.

## Citing
Please cite our paper and/or code as follows:
```tex

@article{verboven2023,
  title={Hydalearn: Highly dynamic task weighting for multitask learning with auxiliary tasks},
  author={Verboven, Sam and Chaudhary, Muhammad Hafeez and Berrevoets, Jeroen and Ginis, Vincent and Verbeke, Wouter},
  journal={Applied Intelligence},
  volume={53},
  number={5},
  pages={5808--5822},
  year={2023},
  publisher={Springer}
}
```
