# Engineering-Novelty-Categorizer-
Classify hardware design descriptions into novelty tiers to assist legal and intellectual property reviewers. The system evaluates performance using macro-averaged F1 score and fine-tunes the text processing pipeline to reduce false positive novelty claims. Aligned with SDG 9: Industry, Innovation and Infrastructure.

The Engineering Novelty Categorizer is a machine learning project that automatically analyzes short hardware design descriptions and classifies them into different novelty tiers. The goal of the system is to help intellectual property (IP) and legal reviewers quickly understand how innovative a hardware design is.

In this project, we follow a simple and interpretable machine learning pipeline rather than complex deep learning models. The dataset contains short patent-style engineering descriptions that represent hardware innovations. Each description is assigned a novelty tier based on how innovative the design appears.

The system processes these design descriptions using Natural Language Processing (NLP) techniques. First, the text is cleaned and converted into numerical features using TF-IDF (Term Frequency–Inverse Document Frequency). These features are then used to train traditional machine learning models such as:

Logistic Regression

Decision Tree

Random Forest

The models learn patterns in engineering language that indicate different levels of novelty. After training, the system predicts the novelty tier of new design descriptions.

To ensure fair evaluation across all novelty categories, the models are evaluated using the Macro F1 Score, which balances precision and recall for each class. This is particularly important because some novelty tiers may have fewer examples in the dataset. 

patent project overview (1)

The final system provides a fast and efficient way to classify engineering design descriptions into novelty tiers, helping reviewers filter and prioritize innovative designs more effectively.
