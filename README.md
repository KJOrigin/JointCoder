<img src="Pictures/title.png" alt="title" border="0">

<p float="left"><img src="https://img.shields.io/badge/python-v3.9+-red"> <img src="https://img.shields.io/badge/pytorch-v2.6+-blue">
   
# JointCoder
This repository provides the official implementation of the paper **“Who Fights Best? Discovering Winning Personality Pairings for LLM Debate Agents”**, including the MBTI-DB framework, personality-conditioned debate prompts, experimental code, evaluation scripts, and released results, enabling reproducible research and further exploration of personality-driven multi-agent debate in large language models.

<img src="Pictures/fig1.png" alt="fig1" width="60%" border="0">

**Figure1**: Overview of the automated ICD coding task. Given patient EHRs, the goal is to jointly predict ICD-10 disease codes and ICD-9-CM-3 procedure codes, where disease and procedure coding are clinically correlated.

## ✨ Overview
<img src="Pictures/main.png" alt="fig2" border="0">

**Figure2**: Overview of the JointCoder framework and the real-world Chinese ICD coding dataset. JointCoder jointly performs ICD-10 disease coding and ICD-9-CM-3 procedure coding through a unified, workflow-aligned multi-stage multi-agent framework.

## 📂 Dataset Sample
<img src="Doc/Pictures/table1.png" alt="table1" border="0">

## 📊 Experiments
<div align="center">
<img src="Pictures/fig3.png" alt="fig3" width="50%" border="0">
</div>

**Figure3**: The top and bottom 10 MBTI personality pairs ranked by their effect sizes on model performance changes relative to the control setting, with models exhibiting low PAS excluded from the analysis.

<div align="center">
<img src="Pictures/fig4.png" alt="fig4" width="50%" border="0">
</div>

**Figure4**: Accuracy comparison across single-agent and multi-agent inference settings, where the single-agent results are averaged over three MBTI personality prompts.

<div align="center">
<img src="Pictures/fig5.png" alt="fig5" width="50%" border="0">
</div>

**Figure5**: The impact of personality pairs on performance varies across models. Some models show effects that are largely skewed toward negative changes, while others exhibit a greater proportion of positive changes. Here, N denotes the number of evaluated personality pairs.

<div align="center">
<img src="Pictures/fig6.png" alt="fig6" width="50%" border="0">

**Figure6**: LLMs exhibit increasingly positive performance effects from personality pairs as model size grows.
</div>

<div align="center">
<img src="Pictures/fig7.png" alt="fig7" width="50%" border="0">
</div>

**Figure7**: Personality pairs in the Math, Business, and Physics domains lead to better performance than those in other domains across models, with models exhibiting low PAS excluded from the analysis.

<div align="center">
<img src="Pictures/fig8.png" alt="fig8" border="0">
</div>

**Figure8**: (a) Lexical density of the personality description is weakly positively correlated with model performance. (b) Personality-question similarity shows a weak to moderate negative correlation with model performance. (c) Prompt perplexity exhibits a weak negative correlation with model performance.

<div align="center">
<img src="Pictures/fig9.png" alt="fig9" border="0">
</div>

**Figure9**: Performance changes for each model (compared with the control prompt) across different personality-pair selection strategies show that all strategies outperform random selection.

**For more detailed experimental results, please [Click here!](Experiment%20Results/README.md)**


## 🌟 Contributions and suggestions are welcome!
