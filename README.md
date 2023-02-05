# ml2_trl_simp
Project Machine Learning 2 - Group 10

This repository contain notebooks to implement reinforcement learning on text simplification. 

- Notebook: `ml2_batchsize_15.ipynb` produces (TRL-simp) models in the report.
- Folder `trl-simp-batch15` contains the configuration and pre-trained TRL-simp model exported after finish training.
- Notebook: `evaluation matrix.ipynb` is for evaluation different models

At the time of this experiment, the Transformer Reinforcement learning (TRL) API in HuggingFace was not updated with method `AutoModelForSeq2SeqLMWithValueHead` for class `model`. Thus, we installed the library using the Github souce code (pip install trl-0.2.1.tar.gz).

Configuration of the PPO Trainer:
- Batch-size: 15
- Learning rate: 5e-4
- Add customization tuning for memory efficient: Learning rate scheduler, pass SGD optimizer (https://github.com/lvwerra/trl/blob/main/docs/source/customization.mdx)

Run logs for the TRL-simp model are available at this link: https://wandb.ai/ml2_g10/trl/runs/v0dcp47v?workspace=user-anhtth

