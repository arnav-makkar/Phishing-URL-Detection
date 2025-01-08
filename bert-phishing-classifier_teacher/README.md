---
library_name: transformers
license: apache-2.0
base_model: google-bert/bert-base-uncased
tags:
- generated_from_trainer
metrics:
- accuracy
model-index:
- name: bert-phishing-classifier_teacher
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# bert-phishing-classifier_teacher

This model is a fine-tuned version of [google-bert/bert-base-uncased](https://huggingface.co/google-bert/bert-base-uncased) on an unknown dataset.
It achieves the following results on the evaluation set:
- Loss: 0.2941
- Accuracy: 0.873
- Auc: 0.952

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0002
- train_batch_size: 8
- eval_batch_size: 8
- seed: 42
- optimizer: Use OptimizerNames.ADAMW_TORCH with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- num_epochs: 10

### Training results

| Training Loss | Epoch | Step | Validation Loss | Accuracy | Auc   |
|:-------------:|:-----:|:----:|:---------------:|:--------:|:-----:|
| 0.4992        | 1.0   | 263  | 0.3864          | 0.807    | 0.914 |
| 0.4029        | 2.0   | 526  | 0.3635          | 0.838    | 0.934 |
| 0.3699        | 3.0   | 789  | 0.4964          | 0.78     | 0.942 |
| 0.3364        | 4.0   | 1052 | 0.3216          | 0.858    | 0.938 |
| 0.3626        | 5.0   | 1315 | 0.3473          | 0.858    | 0.948 |
| 0.3189        | 6.0   | 1578 | 0.2932          | 0.88     | 0.95  |
| 0.3217        | 7.0   | 1841 | 0.2930          | 0.876    | 0.949 |
| 0.3355        | 8.0   | 2104 | 0.3004          | 0.864    | 0.95  |
| 0.3103        | 9.0   | 2367 | 0.2891          | 0.867    | 0.951 |
| 0.2987        | 10.0  | 2630 | 0.2941          | 0.873    | 0.952 |


### Framework versions

- Transformers 4.47.1
- Pytorch 2.3.0+cu121
- Datasets 3.2.0
- Tokenizers 0.21.0
