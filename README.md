# Introduction
This project is going to complete two implementations:
1. Text-prompt visual grounding based on **Segformer** and **OWLv2**
2. Patch-prompt object composition based on **CLIP**
---
# Install
You need to create a python environment fistly, and then run:\
`pip install -r requirements.txt`\
We use python 3.10.4 while developing.

---
# Pipeline
1. Analyze text to find the target and support surface
2. Semantic segmentation for support surface
3. Detect the obstacles
4. Generate Region Of Interest (ROI)
    - Sample candidate within support surface
    - Score and select top k
