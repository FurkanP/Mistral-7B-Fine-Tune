# Mistral 7B Fine-Tuning with LoRA and Quantization

This repository demonstrates how to fine-tune the Mistral 7B model using LoRA (Low-Rank Adaptation) and quantization techniques to optimize model size and efficiency. The goal is to fine-tune the model for instruction-based learning using the databricks-dolly-15k dataset while employing memory-efficient techniques for large language models.

###LoRA (Low-Rank Adaptation)
LoRA is a method that fine-tunes large models efficiently by updating only a small subset of parameters, reducing memory and computation requirements.

###Quantization
Quantization reduces the precision of model weights, making the model smaller and faster, with minimal impact on accuracy.

## Installation
###  1. Running Locally
If you want to run this project on your local machine, follow these steps:
###Prerequisites
Before you begin, ensure you have the following installed:
- Python 3.8+
- `transformers` library
- `datasets` library
- `bitsandbytes` for quantization
- `peft` for LoRA fine-tuning
- `torch` with CUDA enabled (if using a GPU)

To install the required packages, run:

```bash
pip install transformers datasets bitsandbytes peft torch accelerate
```
Clone this repository and install the required dependencies:
```bash
cd $HOME && git clone https://github.com/mistralai/mistral-finetune.git
cd mistral-finetune
pip install -r requirements.txt
```
### 2. Running on Google Colab

You can easily run this project in Google Colab without installing dependencies locally.

#### Open the Colab Notebook

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/FurkanP/Mistral-7B-Fine-Tune/blob/main/mistral_7b_fine_tune.ipynb]

#### Login to Hugging Face

Run the following code in the Colab notebook to log into Hugging Face:

```python
from huggingface_hub import notebook_login
notebook_login()
```

This code will allow you to authenticate your Hugging Face account, ensuring access to the Mistral 7B model and other required resources.
