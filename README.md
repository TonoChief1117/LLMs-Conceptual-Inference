# LLMs-Conceptual-Inference
Code for the paper "Quantifying Conceptual Brittleness: An Evaluation of Large Language Models on Biographical and Occupational Inference." Evaluates LLMs on factual, biographical, and conceptual reasoning using a historical dataset. Includes a 4-step framework to assess robustness in paraphrased contexts and inference accuracy across models.

From Notability Recognition to Conceptual Inference
A Four-Step Methodology for Evaluating LLM Reasoning

This repository contains the code and evaluation framework for the paper:
"Quantifying Conceptual Brittleness: An Evaluation of Large Language Models on Biographical and Occupational Inference"

Abstract: 
This work presents a framework for quantifying the conceptual brittleness of large language models. We propose a four-step methodology of increasing complexity that leverages biographical data to measure how the inferential performance of LLMs deteriorates under syntactic and semantic variations.
To this end, we evaluate tasks involving factual reasoning, biographical inference, and conceptual inference, using a cross-validation repository of notable individuals from 3500 BC to 2018 AD. We evaluated GPT 4.0, GPT 4o, Llama 3-70B, Llama 4-maverick, Gemma 3, DeepSeek V3 and Mistral-8x7B. 
A major limitation identified was the persistent challenge of inferring an entity’s gender, with GPT-4.0 and Mistral-8x7B exhibiting the greatest variability and showing degraded performance when additional context was provided. Results show GPT-4o achieved the highest accuracy in biographical inference, while Llama 3-70B, Gemma 3, and Mistral-8x7B struggled with paraphrased biographies, revealing robustness gaps. A significant limitation emerged in inferring primary occupations: average performance drops of 22\% for GPT-4o, 28\% for Llama 4-Maverick, and 29\% for DeepSeek V3 when comparing original to paraphrased definitions.
In contrast biographical inference tasks showed only a 9.75\% average decrease, suggesting biographical details provide stronger cues than occupational labels. Our findings demonstrate that, although LLMs encode a vast amount of biographical information, they lack robust conceptual representations, particularly in abstract domains such as occupations. Their performance proves fragile when facing minor variations, underscoring a critical gap between superficial knowledge and deeper inferential reasoning.
