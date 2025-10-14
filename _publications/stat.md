---
title: "Skill-Targeted Adaptive Training"
collection: publications
category: conferences
permalink: /publication/stat
citation: "<b>Yinghui He*</b>, Abhishek Panigrahi*, Yong Lin, Sanjeev Arora"
excerpt: "We introduce a new training paradigm, Skill-Targeted Adaptive Training (STAT), which offers a principled path to overcoming SFT saturation and advancing generalization in LLMs."
date: 2025-10-14
venue: "Arxiv preprint"
paperurl: "https://arxiv.org/abs/2510.10023"
---

**_Abstract_**: Language models often show little to no improvement (i.e., "saturation") when trained via vanilla supervised fine-tuning (SFT) on data similar to what they saw in their training set (e.g., MATH). We introduce a new fine-tuning strategy, STAT, to train such a student model by using the metacognition ability of a stronger large language model (LLM) as the teacher. The teacher uses the task dataset to create a list of skills needed for the task, and then labels each data point with its required skills (Didolkar et al., 2024). By monitoring the student's answers, the teacher creates a Missing-Skill-Profile for the student, tracking how often they failed to apply each skill in their responses. We use this idea to build a modified training set in one of two ways. In STAT-Sel, the teacher uses an existing set of training examples but adaptively reweights them according to the Missing-Skill-Profile. In STAT-Syn, the teacher synthesizes additional examples involving missing skills. Across extensive experiments on Llama and Qwen models, our methods yield improvements of up to 7.5% on MATH, whereas SFT provides only limited gains. Furthermore, STAT enhances performance on out-of-distribution benchmarks (e.g., AIME24/25, AMC23, etc.) by an average of 4.6%. Crucially, we find that STAT is complementary to RL via GRPO (Shao et al., 2024): after the model is improved using STAT to address skill gaps, GRPO continues to add further gains. We conclude that skill-targeted adaptive training should broadly improve current training pipelines.
