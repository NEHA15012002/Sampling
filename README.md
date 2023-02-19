# Comparing Sampling Techniques for 5 Machine Learning Models

## Introduction

This project explores the effectiveness of different sampling techniques for creating a balanced dataset for a machine learning model. The dataset used is initially unbalanced, so random over-sampling and under-sampling techniques are used to create a balanced dataset. Five different sampling techniques are then applied to this balanced dataset, and the accuracies of the resulting samples are compared using five different machine learning models.

## Sampling Techniques

The following five sampling techniques were used in this project:

1. **Simple Random Sampling:** In this technique, each member of the population has an equal chance of being selected for the sample. For example, flipping a coin to determine whether to include a person in the sample.

2. **Stratified Sampling:** This method divides the population into homogeneous groups called strata and then randomly samples from each stratum. This ensures that each group is well-represented in the sample. For example, selecting a certain number of people from each age group or gender.

3. **Systematic Sampling:** In this technique, the population is first arranged in some order, such as alphabetical or numerical order. A starting point is then randomly selected, and every nth member of the population is selected for the sample. For example, selecting every 10th name on a list.

4. **Cluster Sampling:** Cluster sampling involves dividing the population into clusters and then randomly selecting clusters to sample. This method is useful when the population is large and dispersed. For example, selecting a random city block and then sampling all households within that block.

5. **Convenience Sampling:** This technique involves selecting individuals who are readily available and willing to participate in the study. This method is often used in pilot studies or exploratory research, but it may not be representative of the entire population. For example, asking people in a shopping mall to participate in a survey.

## Comparison Table

The table below shows the accuracies of each sampling technique on five different machine learning models. The dataset used for all models is a balanced version of the original unbalanced dataset using random over-sampling and under-sampling techniques.

| Sampling Technique | Decision Tree | SVM | Logistic Resgression | KNN | Naive Bayes |
|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|
| Simple Random Sampling | 0.9778 | 0.8954 | 0.8917 | 0.8915 | 0.7275 |
| Systematic Sampling | 0.9813 | 0.8989 | 0.9213 | 0.9493 | 0.6854 |
| Stratified Sampling | 0.9851 | 0.8937 | 0.9217 | 0.9498 | 0.6890 |
| Cluster Sampling | **0.9868** | 0.9000 | 0.9088 | 0.9691 | 0.9235 |
| Convenience Sampling | 0.9849 | 0.9190 | 0.9322 | 0.9623 | 0.7740 |

Best: Cluster Sampling

Worst: Simple Random Sampling

## Conclusion

It is recommended to use cluster sampling for this dataset, as it consistently gives the best performance across all models. However, other sampling techniques may be worth considering for different datasets or models.
