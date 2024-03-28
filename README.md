# Analysing Adversarial Attacks on Tabular Data Classifiers

Guaranteeing the security of Machine Learning (ML) classifiers is a crucial priority of all institutions
employing automatic decision-making systems, to protect their businesses against cyberattacks and
fraudulent attempts. 

Adversarial attacks are novel techniques that, other being proven to be effective
to fool image classification models, can also be applied to tabular data. Adversarial attacks aim
at producing adversarial examples, in other words, slightly modified inputs that induce the Artificial
Intelligence (AI) system to return incorrect outputs that are advantageous for the attacker. 

To illustrate
the threat of adversarial attacks in a tabular context, we consider the scenario where a bank customer
applies for a loan. A machine learning model is used to make a decision regarding the acceptance of
the application based on customer provided information (incomes, age, etc.). The model advises the
bank to reject the application of our customer. However, he is determined to get the loan by filling
false information to mislead the model.
The key for this attack to succeed is its imperceptibility: the
application should remain credible and relevant, in coherence with the model’s prediction. An adversarial 
attack must create adversarial samples xadv that are sufficiently close to the
real data x, i.e., |x − xadv |2 < ϵ, where ϵ is that maximum distance to which an attack is considered
credible.

This repository explores the impact of adversarial attacks on tabular data
classifiers, specifically within the context of loan risk prediction using the **German Credit Risk** dataset. 

# :pushpin: Jupyter Notebook structure
### 1. Data Exploration and Preprocessing
- Data Preprocessing
- Exploratory Data Analysis
### 2. Unsupervised Exploration and Clustering
- Dimensionality Reduction for data visualization (PCA and t-SNE)
- Unsupervised Data Analysis (K-Means and GMM clustering, purity assessment)
### 3. Supervised Data Analysis
- Classifier Selection (LogReg, RF, SVM, CNB, NN)
- Cross Validation 
- Classifier Evaluation
### 4. Adversarial Attacks and Countermeasure Exploration
- Random Noise Attack
- Feature Specific Noise Attack
- Adversarial Attacks: 
  - **FGSM**
  - **PGD** (Untargeted/Targeted PGD - L2/Linf)
  - **DeepFool**
  - **HopSkipJump**
- Adversarial Defenses: 
  - **Adversarial Training**
  - **Gradient Obfuscation**
  - **Data Sanitization**

