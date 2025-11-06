# CAAL

The implementation of the paper **"Cross-Modal Inconsistency in Clustering: A Confidence-Aware Active Learning Framework"**. The code is coming soon.

## Context

In multimodal data clustering, one commonly overlooked challenge is the presence of **inconsistent semantic information** across different modalities. This inconsistency can significantly affect the overall clustering accuracy. Unsupervised methods, such as contrastive learning, often struggle to correctly distinguish the true categories of these samples due to the lack of prior knowledge.

## Example of Inconsistent Semantic Information

Below is an example showcasing inconsistent semantic information across different modalities:

![Inconsistent Examples](https://github.com/shichenhui/CAAL/blob/main/inconsistent_examples.png)

## Challenging Samples: A Critical Bottleneck

Challenging samples represent a critical bottleneck for improving accuracy in unsupervised multimodal clustering. These difficult cases can be divided into two categories:

- **Semantically inconsistent samples**: These samples have conflicting signals across modalities, preventing accurate categorization.
- **Samples with low-quality modalities**: These exhibit poor quality in some modalities, which further complicates the clustering process.

It is important to note that **modal consistency** strongly correlates with **discriminability**. When a modality exhibits low agreement with others, it typically demonstrates low confidence. Although obtaining modal agreement information is relatively straightforward in unsupervised settings, distinguishing the correct modalities for inconsistent samples remains challenging.

## Proposed Approach

In this context, providing the model with a **limited but strategically selected set of labeled instances** can substantially improve model performance. Therefore, this paper proposes the **Confidence-Aware Active Learning (CAAL)** framework to enhance multimodal clustering.

## Performance Comparison

The table below compares the clustering performance of our method with state-of-the-art techniques:

![Performance Comparison](https://github.com/shichenhui/CAAL/blob/main/accuracy_table.png)

## Confidence Distribution

The figure below shows the distribution of **unlabeled confidence** and **labeled confidence** across five datasets:

![Confidence Distribution](https://github.com/shichenhui/CAAL/blob/main/confidence2.png)

## Conclusion

The confidence distribution in the figure above clearly demonstrates the feasibility and effectiveness of our confidence-aware method. This indicates that the proposed approach has significant **practical application value** in improving the accuracy of unsupervised multimodal clustering.
