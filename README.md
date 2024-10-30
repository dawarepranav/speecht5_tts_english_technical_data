| :label: **PAGE**                   | :page_facing_up: **LINK**                                                                             |                        
|-------------------------------------|------------------------------------------------------------------------------------------------------|                   
| **MARATHI TTS GITHUB LINK  LINK**                | [MARATHI TTS REPO](https://github.com/dawarepranav/speechT5_marathi_finetuned-)         |
| **HUGGING FACE ENG TECHNICAL DATA**   | [HUGGING FACE TECHNICAL DATA  ](https://huggingface.co/pranavdaware/speecht5_tts_technical_train2) |
| **HUGGING FACE MARATHI TTS**          | [HUGGING FACE MARATHI TTS ](https://huggingface.co/pranavdaware/speecht5_tts_marathi_train2)       |
| **REPORT**                            | [REPORT](https://huggingface.co/pranavdaware/speecht5_tts_marathi_train2)                          |










| :label: **Field**        | :page_facing_up: **Description**                     |                                   
|--------------------------|-----------------------------------------------------|                                        
| **📚 Library Name**       | `transformers`                                      |
| **🌐 Language**           | `en`                                                |
| **📄 License**            | `mit`                                               |
| **🛠️ Base Model**         | `microsoft/speecht5_tts`                            |
| **🏷️ Tags**               | `generated_from_trainer`                            |
| **📊 Datasets**           | `custom`                                            |
| **🔍 Model Index**        | **SpeechT5 TTS technical train2**                   |

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# 🎤 SpeechT5 TTS Technical Train2

This model is a fine-tuned version of [microsoft/speecht5_tts](https://huggingface.co/microsoft/speecht5_tts) using a custom dataset, specifically trained for *Text-to-Speech (TTS)* tasks. 

🎯 *Key Metric:*
- *Loss* on the evaluation set: 0.3763

📢 *Listen to the generated sample:*

  The text is " Hello ,few technical terms i used while fine tuning are  API and REST and CUDA and TTS."

<audio controls src="https://cdn-uploads.huggingface.co/production/uploads/66f64964584cae45b5494560/JYJmDNPHnBRLuvqGTJQSu.wav"></audio>

---

## 📝 Model Description

The *SpeechT5 TTS Technical Train2* is built on the *SpeechT5* architecture and was fine-tuned for speech synthesis (TTS). The fine-tuning focused on improving the naturalness and clarity of the generated audio from text.

🛠 *Base Model*: [Microsoft SpeechT5](https://huggingface.co/microsoft/speecht5_tts)  
📚 *Dataset*: Custom (specific details to be provided)

---
## Fine-Tuning Code

The fine-tuning code is available in the following Jupyter Notebook:

**[SpeechT5 TTS Fine-Tuning Code](https://github.com/dawarepranav/speecht5_tts_english_technical_data/blob/main/train2_TECHNICAL_TERMS__SpeechT5_TTS_Fine_tuning_%20(1).ipynb)**

This notebook includes:
- Model setup and configuration.
- Loading the technical vocabulary dataset.
- Training and optimization steps for enhanced pronunciation of technical terms.

  
## 🔧 Intended Uses & Limitations

### ✅ *Primary Use Cases:*
- *Text-to-Speech (TTS)* for technical Interview Texts .
- *Virtual Assistants*:
  

### ⚠ *Limitations:*
- Best suited for English TTS tasks.
- Require further fine-tuning on Large dataset  .

---

## 📅 Training Data

The model was fine-tuned on a *custom dataset*, curated for enhancing TTS outputs. This dataset consists of various types of text that help the model generate more natural speech, making it suitable for TTS applications.

### ⚙ *Hyperparameters:*

The model was trained with the following hyperparameters:

- *Learning Rate*: 1e-05
- *Train Batch Size*: 16
- *Eval Batch Size*: 8
- *Seed*: 42
- *Gradient Accumulation Steps*: 2
- *Total Train Batch Size*: 32
- *Optimizer*: AdamW (betas=(0.9, 0.999), epsilon=1e-08)
- *LR Scheduler Type*: Linear
- *Warmup Steps*: 50
- *Training Steps*: 500
- *Mixed Precision Training*: Native AMP

### ⚙ *📊 Training Results:*:
| 🏋‍♂ Training Loss | 🕑 Epoch | 🛤 Step | 📉 Validation Loss |
|:-------------------:|:-------:|:-------:|:-----------------:|
|        1.1921       | 100.0   | 100     |      0.4136       |
|        0.8435       | 200.0   | 200     |      0.3791       |
|        0.8294       | 300.0   | 300     |      0.3766       |
|        0.7959       | 400.0   | 400     |      0.3744       |
|        0.7918       | 500.0   | 500     |      0.3763       |


### 📦 Framework Versions

- *Transformers*: 4.46.0.dev0
- *PyTorch*: 2.4.1+cu121
- *Datasets*: 3.0.2
- *Tokenizers*: 0.20.1
