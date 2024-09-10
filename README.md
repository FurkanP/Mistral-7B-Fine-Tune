Mistral 7B Fine-Tuning with LoRA and Quantization

This repository demonstrates how to fine-tune the Mistral 7B model using LoRA (Low-Rank Adaptation) and quantization techniques to optimize model size and efficiency. The goal is to fine-tune the model for instruction-based learning using the databricks-dolly-15k dataset while employing memory-efficient techniques for large language models.

Installation

Before you begin, ensure you have the following installed: Python 3.8+ transformers library datasets library bitsandbytes for quantization peft for LoRA fine-tuning torch with CUDA enabled (if using a GPU)

To install the required packages, run:
pip install transformers datasets bitsandbytes peft torch accelerate

Usage in Google Colab

You can easily run this project in Google Colab without installing dependencies locally.

Open the Colab Notebook Click here to open the Colab notebook.

Login to Hugging Face

Run the following code in the Colab notebook to log into Hugging Face:

from huggingface_hub import notebook_login
notebook_login()

This code will allow you to authenticate your Hugging Face account, ensuring access to the Mistral 7B model and other required resources.
