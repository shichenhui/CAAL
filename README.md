# CAAL
The implementation of "Cross-Modal Inconsistency in Clustering: A Confidence-Aware Active Learning Framework"

In the clustering of multimodal data, a prevalent yet commonly overlooked phenomenon is that certain samples exhibit inconsistent semantic information across different modalities, which adversely affects the overall clustering accuracy. Unsupervised methods such as contrastive learning and others are struggling to correctly distinguish the true categories of these samples since the absence of prior knowledge.

An example that with inconsistent semantic information across modalities:

<img src="https://github.com/shichenhui/CAAL/blob/main/inconsistent_examples.png" width="500px">

Challenging samples represent a critical bottleneck for improving accuracy in unsupervised multimodal clustering. These difficult cases include both semantically inconsistent samples with conflicting modal signals that prevent accurate categorization, and samples exhibit low quality in some modalities.
It is noteworthy that the consistency between a sample's modalities strongly correlates with its discriminability. When a modality exhibits low agreement with other modalities, it typically also demonstrates low confidence. While obtaining modal agreement information is relatively straightforward in unsupervised settings, distinguishing which modalities are correct remains challenging for inconsistent samples.

In this context, providing the model with a limited but strategically selected labeled instances can substantially improve model performance. Therefore, this paper proposes a **Confidence-Aware Active Learning framework (CAAL)** to further boost multimodal clustering.


