---
layout: post
title: Linked Fusion
subtitle: Interpretation of Observations
---


In the context of LinkedFusion, the goal is to extract the smallest building blocks from observations that compose a scene. These building blocks, which may not necessarily be structural elements, represent the minimal segments required for coherent objects. This mathematical problem involves maximizing the conditional probability of a set of segmentations based on feature inputs, such as XYZ coordinates and color information for point clouds, or pixel values for images.

![Segmentation](../assets/img/segmentation.PNG)

Currently, each modality (point clouds and images) is processed independently, leading to specific interpretation models for each. While this approach is common, it has limitations, especially in domains like construction, where objects vary in texture and geometric features. Achieving market adoption rates of around 90% necessitates combining these approaches, prompting the key question of how to fuse them effectively.


