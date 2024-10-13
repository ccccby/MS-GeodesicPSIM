# [MS-GeodesicPSIM: Predicting the Quality of Static Mesh with Texture Map via multi-scale Geodesic Patch Similarity (MM Asia 2024)]

by Bingyang Cui, Yujie Zhang, Qi Yang, Yiling Xu

This respository is about a full-reference textured mesh quality metric based on the multi-scale Geodesic Patch Similarity. The key idea is that **human vision perceives real-world objects with multi-scale characteristics. The human visual system (HVS) provides different feedback for the same object when viewed from varying distances**.

## Introduction
![image text](https://github.com/ccccby/MS-GeodesicPSIM/blob/main/figure/framework.jpg)

We propose a multi-scale MQA metric that aligns well with the HVS. Considering that as the viewing distance increases, the textured mesh loses some visual details, we employ a novel mesh simplification method that integrates three effective guiding features into the traditional quadric error metric (QEM) to create a multi-scale mesh representation. We then extend the GeodesicPSIM metric into the multi-scale version, called MS-GeodesicPSIM. Specifically, for a textured mesh, we first apply the proposed simplification method to obtain meshes in different scales. After calculating the GeodesicPSIM scores for each scale, we aggregate these scores to produce the overall MS-GeodesicPSIM score. This approach allows the metric to capture finer details, resulting in more accurate and reliable quality prediction.

## Demo

The code is coming soon.

## Results
- Datasets
1. [TSMD](https://multimedia.tencent.com/zh/resources/tsmd)
2. [SJTU-TMQA](https://ccccby.github.io/)
3. [YANA](https://yananehme.github.io/publications/2022-ACM-TOG)

- Quantitative comparison
![image text](https://github.com/ccccby/MS-GeodesicPSIM/blob/main/figure/performance.png)
