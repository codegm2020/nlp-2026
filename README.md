Sanskrit Sandhi Segmentation using ByT5
This project implements Sanskrit word segmentation using a byte-level Transformer.

Overview
Sanskrit combines words using sandhi rules, which remove word boundaries and modify characters. This notebook models sandhi splitting as a sequence-to-sequence task.

Example: Input: वृिद्धरादैच्
Output: वृिद्धः+आदैच्

Approach
Model: google/byt5-base
Framework: Hugging Face Transformers
Task: Sequence-to-sequence generation
Dataset: SandhiKosh
Training Details
Epochs: 10
Learning rate: 1e-4
Batch size: 8
Max sequence length: 256
Results
ByT5 Accuracy: 84.67%
Lookup Baseline: 72.44%
No-split Baseline: 0%
The model learns generalizable sandhi transformations beyond memorization.

How to Run
Open the notebook and run all cells.
