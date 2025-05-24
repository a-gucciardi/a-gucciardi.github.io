---
title: Self-rewarding LLM, LoRA and a few VLMs
description: LLM fine-tuning, text-to-image, and automated self-supervision
date: 2024-08-24 
links:
  - title: Paper 
    description: 
    website: https://arxiv.org/pdf/2405.13473
    image: https://arxiv.org/static/browse/0.3.4/images/icons/smileybones-pixel.png
  - title: GitHub Repo
    description: Codebase is open-source and available on GitHub.
    website: https://github.com/safouaneelg/SRT2I
    image: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
weight: 3
image: 

---
<!-- ## Tech -->
> [**LLM Fine-Tuning**] **[LoRA]** **[Diffusion]** **[Self-Supervised]** **[SelfRewarding]** **[PyTorch]** **[HuggingFace]**


## Highlights

* Fine-tuned Stable Diffusion using a self-generated, self-evaluated dataset.

* Incorporated LLM with automated reward modeling and prompt-following accuracy.

* Achieved a 60% performance improvement after training over the base text-to-image models.

* Enabled fully automated training loops, reducing the need for manual annotations.

## Ideas
<!-- By guiding LLMs to self-assess and follow their own learning process, we tried to see how models do beyond reliance on human feedback.  
Our contribution builds on the LoRA concept and expands it to the text-to-image (diffusion) models. -->
This project sits at the intersection of LLM fine-tuning, multi-modal AI, and automated self-supervision.  
We showcase a pipeline of scalable AI systems that learn and improve independently.

The core idea? We developed and fine-tuned a self-rewarding system for generative models to automatically curate and score their own training data. Using a combination of object detection, image captioning, and language model judgment, the model learns to evaluate its outputs and iteratively improve based on its own assessments. 
This significantly streamlines the training process and enhances data quality, enabling highly targeted and user-specific improvements in image generation.

![Some fun and insights with LoRA levels](lora.png)

## My Thoughts

> * It was a lot of fun to retrain text to image models and prompts, and see some models evaluate some other models.
> * Potentially replaces Reinforcement Learning with Human Feedback, **if** we reach the point where we trust the LLM/VLM for evaluation. (will we ever? ) 
> * The idea of the pipeline stills stands and is something I would love to get back to with new models
 **Prompts -> Text-to-Image -> Self-Eval + Filtering -> Fine-tuning**
