# CrossMac2025 
[Update: September 7, 2025]

──────────────────────────────
Note on MAE:
The MAE reported in the paper is computed on hard-mapped discrete labels 
(i.e., mapping predicted classes back to {-3,…,+3} before evaluation). 
Therefore, this MAE value should be interpreted as a reference indicator 
and has only limited comparability with MAE values reported in prior work 
that use fully continuous labels.
──────────────────────────────
Note on F1:
The F1 score reported in the paper corresponds to the binary-F1 variant as implemented here. 
After submission, we realized that this is different from the weighted-F1 metric commonly used in prior work. 
We will update the results in our revision for consistency.
──────────────────────────────

Important Note:In our ablation studies, we did not simply remove the ablated modality. Instead, we adopted a structurally symmetric replacement strategy to ensure fair comparison across different settings. Specifically, when ablating the audio modality, we used the Vision-to-Text and Text-to-Vision paths (V→T, T→V). When ablating the text modality, we employed Audio-to-Vision and Vision-to-Audio paths (A→V, V→A); and when ablating the visual modality, we adopted Audio-to-Text and Text-to-Audio paths (A→T, T→A). This design ensures that the number of attention paths and the fusion strategy remain consistent with the full model configuration.

The released code is intended for reproducing the results reported in our paper "CrossMAC: Cross-Modal Attention Contrastive Mechanism for Enhanced Multimodal Sentiment Analysis". All hyperparameters used in the code are consistent with those described in the paper.

The experiment code for CMU-MOSI is available at https://github.com/HXlilith369/test1, with minor parameter differences compared to the main CMU-MOSEI experiments.


