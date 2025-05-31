# LLMs-Conceptual-Inference
Code for the paper "From Notability Recognition to Conceptual Inference." Evaluates LLMs on factual, biographical, and conceptual reasoning using a historical dataset. Includes a 4-step framework to assess robustness in paraphrased contexts and inference accuracy across models.

From Notability Recognition to Conceptual Inference
A Four-Step Methodology for Evaluating LLM Reasoning

This repository contains the code and evaluation framework for the paper:
"From Notability Recognition to Conceptual Inference: A Four-Step Methodology for Evaluating LLM Reasoning."

Overview
This project introduces a structured methodology to assess the reasoning capabilities of Large Language Models (LLMs) across three key tasks:

Factual reasoning

Biographical inference

Conceptual inference

The evaluation is based on a historically rich, cross-validated dataset of notable individuals spanning from 3500 BC to 2018 AD. This dataset supports inquiries grounded in social science—such as gender, economic growth, and cultural development—providing a unique context for evaluating LLM behavior across diverse temporal and cultural settings.

Methodology
The evaluation framework follows a four-step pipeline:

Selection and filtering of individuals using a notability index

Querying contextual and non-contextual biographical information

Identity inference from original and paraphrased biographies

Occupation inference using original and paraphrased role definitions

Benchmark Models
We benchmarked the following LLMs:

GPT-4.0

LLaMA 3-70B

Mistral 8x7B

Key Findings
LLaMA 3-70B performed strongly in biographical inference.

Mistral 8x7B showed sensitivity to paraphrased inputs.

GPT-4.0 achieved the highest accuracy across all tasks.

A notable finding is the significant 31.5% drop in performance for occupation inference when using paraphrased definitions, compared to only 4.26% for biographical inference. This suggests that LLMs handle surface-level paraphrasing better in factual contexts than in more abstract conceptual tasks.

Conclusion
Our study highlights limitations in how current LLMs represent complex social roles and conceptual categories. These insights underscore the challenges LLMs face in achieving human-level inference in real-world, socially grounded tasks.
