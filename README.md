<img src="Pictures/title.png" alt="title" border="0">

<p float="left"><img src="https://img.shields.io/badge/python-v3.9+-red"> <img src="https://img.shields.io/badge/pytorch-v2.6+-blue">
   
# JointCoder
This repository provides the official implementation of the paper **“JointCoder: Exploring Automated ICD Coding on Real-World Chinese EHRs with a Multi-Agent Framework”** , including a real-world Chinese ICD dataset and a workflow-aligned multi-agent framework for joint ICD-10 disease and ICD-9-CM-3 procedure coding.

<div align="center">
   <img src="Pictures/fig1.png" alt="fig1" width="80%" border="0">
</div>

**Figure 1**: Overview of the automated ICD coding task. Given patient EHRs, the goal is to jointly predict ICD-10 disease codes and ICD-9-CM-3 procedure codes, where disease and procedure coding are clinically correlated.

## ✨ Overview
<img src="Pictures/main.png" alt="fig2" border="0">

**Figure 2**: Overview of the JointCoder framework and the real-world Chinese ICD coding dataset. JointCoder jointly performs ICD-10 disease coding and ICD-9-CM-3 procedure coding through a unified, workflow-aligned multi-stage multi-agent framework.

## 🌐 JointCoder System Features
The system provides four core functions:

1. **Select Demo Cases**  
   Users can choose from four preloaded EHR samples (Sample 4 contains no surgical record). The system performs OCR-based content extraction and de-identification, allows content review and editing, and then runs disease and procedure coding in parallel. Agent outputs are expandable/collapsible, and final ICD results are displayed in tables and saved to the database.

2. **Upload a Single PDF File**  
   Users can upload a local PDF EHR file. The system applies OCR and de-identification, supports content editing before submission, and performs parallel disease and procedure coding with structured result display.

3. **Batch Upload PDF Files**  
   Multiple PDF EHR files can be uploaded simultaneously. The system processes each case sequentially, applies batch OCR, and performs parallel coding for each case. Results are displayed in tables and stored in the database.

4. **Upload Excel and Batch Submit**  
   Users can upload de-identified Excel-formatted EHR files directly (without OCR), significantly improving efficiency. The system processes each case sequentially and performs parallel coding with structured output.
   
After coding, users can provide case-level or result-level feedback, mark cases as completed, and export coding results or feedback data.

These features are fully demonstrated in the demo video. **Demo video: [YouTube link](https://www.youtube.com/watch?v=fC23ge_EK3E).**

<img src="Pictures/screenshot.png" alt="screenshot" border="0">
<div align="center">
   
**Figure 3**: Screenshot of the web-based JointCoder system interface.
</div>

## 🎬 Demo Video
**Demo video: [YouTube link](https://www.youtube.com/watch?v=fC23ge_EK3E).**

We provide a demo video (2 minutes and 29 seconds) that comprehensively showcases all functionalities of **JointCoder**.
The video demonstrates the complete workflow, including demo case selection, OCR-based content extraction and de-identification, editable input review, parallel disease and procedure coding, expandable multi-agent outputs, structured ICD result presentation, feedback annotation, and data export.

## 📂 Dataset Sample
We construct a real-world dataset for automated ICD coding based on de-identified patient EHRs from a top-tier Chinese hospital. The dataset contains 6,747 hospitalization records, each annotated with ICD-10 disease codes and ICD-9-CM-3 procedure codes by experienced coders.﻿
To illustrate the structure and format of the dataset, we provide six representative sample records in **Dataset Sample/Dataset Samples.xlsx.**

## 📊 Experiments
<div align="center">
<img src="Pictures/fig41.png" alt="fig41" width="70%" border="0">
</div>

**Figure 4**: Performance of different methods on the proposed ICD coding dataset. Models marked with $^\dagger$ denote commercial APIs. The best and second-best results are highlighted in **bold** and <ins>underline</ins>, respectively. Results marked with $^*$ indicate statistically significant improvements over the strongest baseline ($p < 0.05$).

## 📌 Case Study
<div align="center">
<img src="Pictures/case1.png" alt="case1" width="70%" border="0">

**Figure 5**: Case study comparing disease and procedure ICD prediction results of different methods on a real-world Chinese EHR example.
</div>

## 🧪 Ablation Study
<div align="center">
<img src="Pictures/fig5.png" alt="fig5" width="50%" border="0">

**Figure 6**: Ablation results for disease ICD coding.
</div>
<div align="center">
<img src="Pictures/fig6.png" alt="fig6" width="50%" border="0">

**Figure 7**: Ablation results for procedure ICD coding.
</div>

## 🧩 Workflow Example
<div align="center">
<img src="Pictures/workflow1.png" alt="workflow1" width="80%" border="0">
</div>

**Figure 8**: An illustrative example of the JointCoder workflow, showing intermediate outputs for disease and procedure coding at each stage.

## 📖 Citation

If you find this repository or our work useful, please cite our paper:

```bibtex
@inproceedings{liu2026jointcoder,
  title     = {JointCoder: Exploring Automated ICD Coding on Real-World Chinese EHRs with a Multi-Agent Framework},
  author    = {Liu, Kangjun and Li, Zhenyu and Wang, Jianlei and Guan, Hongjiao and Lian, Ying and Chen, Guoqiang},
  booktitle = {Proceedings of the 64th Annual Meeting of the Association for Computational Linguistics: System Demonstrations},
  year      = {2026}
}
```

## 🌟 Contributions and suggestions are welcome!
