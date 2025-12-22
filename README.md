# Semantic_Drift_Detection
[CVPR'25] LogSAD: Towards Training-free Anomaly Detection with Vision and Language Foundation Models

## Main Method 



## TODO
- Replace hard-coded, product-specific inspection codes inside the histogram functions with a more general and configurable implementation.
- Implement the match-of-thought procedure for semantic consistency evaluation.
- Unify backbone selection across product classes in patch matching.
    Currently:
  - *pushpins*, *screw_bag*: CLIP
  - *splicing_connectors*, *breakfast_box*, *juice_bottle*: DINOv2
- Add evaluation scripts for standard visual anomaly detection benchmarks, including **MVTecAD** and **VisA**.
