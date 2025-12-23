# Semantic_Drift_Detection
[CVPR'25] LogSAD: Towards Training-free Anomaly Detection with Vision and Language Foundation Models

## Main Method 


The proposed framework consists of three components: 
- **Patch Matching**
- **Interest Matching**
- **Composition Matching**

Patch matching and interest matching are implemented in the `forward_one_sample` function of `model_ensemble_few_shot.py`.

Composition matching is implemented in the `histogram` function of `model_ensemble_few_shot.py`.


## TODO
- [ ] Replace hard-coded, product-specific inspection codes inside the histogram functions with a more general implementation.
- [ ] Implement the **match-of-thought** procedure for semantic consistency evaluation.
- [ ] Unify backbone selection across product classes in patch matching.


  - Currently:
    - *pushpins*, *screw_bag*: CLIP
    - *splicing_connectors*, *breakfast_box*, *juice_bottle*: DINOv2
- [ ] Add evaluation scripts for standard visual anomaly detection benchmarks, including **MVTecAD** and **VisA**.


## Dependencies and References

This project is built on top of the `anomalib` framework.
For the original implementation and related utilities, please refer to:

- https://github.com/zhang0jhon/LogSAD/tree/master/anomalib
