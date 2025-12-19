**MEARN: Enhancing B-cell Epitope Prediction with ESM-Derived Protein Embeddings and an Attention–Residual Neural Network**

B-cell epitopes are key targets in vaccine design and therapeutic antibody development, yet accurate prediction remains challenging due to severe class imbalance, high sequence heterogeneity, and limited experimentally validated data. These issues often lead to biased learning and poor generalization in conventional deep learning models.

To address these challenges, we propose MEARN, an Attention–Residual Neural Network that leverages semantically rich protein embeddings from the ESM protein language model. MEARN integrates multi-head attention with residual MLP blocks and Layer Normalization to capture latent feature interactions, stabilize training, and enhance representation learning under imbalanced data conditions.

Experimental results demonstrate that MEARN achieves strong and balanced performance in B-cell epitope prediction (ACC = 0.9287, AUC = 0.8092, BAC = 0.7345, MCC = 0.4983, PR-AUC = 0.4948), confirming the effectiveness of combining ESM embeddings with an attention–residual architecture.

Overall, MEARN provides a robust and extensible framework for biological sequence analysis and offers valuable methodological insights for future research in bioinformatics and computational immunology
