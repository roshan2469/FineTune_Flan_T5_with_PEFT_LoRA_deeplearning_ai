# Parameter-Efficient Fine-Tuning of FLAN-T5 using LoRA
Overview

This project demonstrates parameter-efficient fine-tuning of FLAN-T5 using LoRA (Low-Rank Adaptation) through the PEFT framework.

The goal is to reduce computational cost while achieving strong downstream task performance.


Key Concepts

> Instruction tuning

> Parameter-efficient fine-tuning (PEFT)

> Low-rank matrix adaptation

> Reduced memory footprint training

> Task-specific adaptation without full model retraining


Technical Stack

> Python

> PyTorch

> Hugging Face Transformers

> PEFT (Parameter Efficient Fine-Tuning)

> Datasets

Architecture

> Base model: FLAN-T5 (encoder-decoder transformer)

> LoRA layers injected into attention modules

> Frozen base weights

> Trainable low-rank matrices


Why LoRA?

> Traditional fine-tuning updates all parameters, which is:

> Expensive

> Memory intensive

> Slow for large models

LoRA:

> Freezes original weights

> Adds small trainable adapters

> Achieves competitive performance

> Significantly reduces GPU requirements


Outcomes

> Reduced training time

> Minimal memory usage

> Comparable task accuracy

> Scalable adaptation strategy



Production Applications

> Enterprise NLP systems

> Resource-constrained fine-tuning

> Multi-task model deployment

> Rapid experimentation pipelines
