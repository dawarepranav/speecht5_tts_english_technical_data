---
library_name: transformers
language:
- en
license: mit
base_model: microsoft/speecht5_tts
tags:
- generated_from_trainer
datasets:
- custom
model-index:
- name: 'SpeechT5 TTS technical train2 '
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# SpeechT5 TTS technical train1 

This model is a fine-tuned version of [microsoft/speecht5_tts](https://huggingface.co/microsoft/speecht5_tts) on the custom dataset.
It achieves the following results on the evaluation set:
- Loss: 0.3763

SAMPLE TEXT : "hello ,few technical terms i used while fine tuning are  API and REST and CUDA and TTS."
<audio controls src="https://cdn-uploads.huggingface.co/production/uploads/66f64964584cae45b5494560/JYJmDNPHnBRLuvqGTJQSu.wav"></audio>

  

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 1e-05
- train_batch_size: 16
- eval_batch_size: 8
- seed: 42
- gradient_accumulation_steps: 2
- total_train_batch_size: 32
- optimizer: Use adamw_torch with betas=(0.9,0.999) and epsilon=1e-08 and optimizer_args=No additional optimizer arguments
- lr_scheduler_type: linear
- lr_scheduler_warmup_steps: 50
- training_steps: 500
- mixed_precision_training: Native AMP

### Training results

| Training Loss | Epoch | Step | Validation Loss |
|:-------------:|:-----:|:----:|:---------------:|
| 1.1921        | 100.0 | 100  | 0.4136          |
| 0.8435        | 200.0 | 200  | 0.3791          |
| 0.8294        | 300.0 | 300  | 0.3766          |
| 0.7959        | 400.0 | 400  | 0.3744          |
| 0.7918        | 500.0 | 500  | 0.3763          |


### Framework versions

- Transformers 4.46.0.dev0
- Pytorch 2.4.1+cu121
- Datasets 3.0.2
- Tokenizers 0.20.1
