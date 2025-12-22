# Overview

This repository contains the source code, datasets, and experimental pipelines for an Honours project comparing traditional transformer architectures (BERT) with modern Large Language Models (Llama 3.1 8B and Mistral 7B) in the context of misinformation detection

# Repo structure
├── Untrained_data_llama_3.ipynb          # Phase 1: Zero-shot and Few-shot testing scripts

├── finetune_llama.ipynb          # Phase 2: Fine-tuning and post-performance tests

# Methodology: 2 Phases

## Phase 1: Baseline & Prompting (Untrained_data_llama_3.ipynb)

We evaluate "out-of-the-box" knowledge of Llama 3.1 8B across the LIAR, Pheme and ISOT_Politics.

Zero-Shot: Testing the model's ability to classify news articles based solely on pre-trained weights.
Few-Shot (N-Shot): Add (x - x can be changed) labeled examples into the context window to measure the impact of In-Context Learning (ICL) on detection accuracy.

## Phase 2: Optimization & Fine-Tuning (finetune_llama.ipynb)
This phase documents the supervised adaptation of the model using Parameter-Efficient Fine-Tuning (PEFT).

Fine-Tuning Technique: 4-bit QLoRA (Quantized Low-Rank Adaptation).

Checkpoints: Training was conducted across multiple epochs. The resulting weights for Epoch 1 and Epoch 2 are hosted on Google Drive (link included in the files) due to GitHub file size limits.

# Environment Setup

This project is optimized for execution in Google Colab using NVIDIA T4 (Zero-shot and few-shots), L4 (Few-shots and finetune) and A100 (finetune) GPUs.
All necessary component to run the code is included in the .ipynb file provided
