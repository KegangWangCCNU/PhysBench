# PhysBench
A large-scale training and benchmarking framework for rPPG.

Full release coming soon.

## What's new? 
* The training and testing code, refactored using Keras and JAX, is fully just-in-time (JIT) compiled. All models support FP16 mixed precision acceleration and Distributed Data Parallel (DDP), and can be deployed in both single-node multi-GPU environments and multi-node multi-GPU environments (under testing).
* A more flexible data loader that offers sub-dataset filtering capabilities, asynchronous streaming loading at speeds up to 4GB/s, and achieves nearly 100% GPU utilization. 
* Optimized APIs facilitate the addition of custom models and the application of data augmentation algorithms during training.

## In progress......
* Large-scale self-supervised pre-training for rPPG, supporting clusters of tens to hundreds of A100/H100.
* Multi-task fine-tuning using rPPG models to predict additional signals such as blood pressure (BP) and blood oxygen (SpO2).
* Continuous replication and benchmarking of state-of-the-art (SOTA) end-to-end models.
* Development documentation and function comments for beginners.

## Related works
* [A Plug-and-Play Temporal Normalization Module for Robust Remote Photoplethysmography](https://github.com/KegangWangCCNU/TemporalNormalization/tree/main)

The complete code is being organized. If you wish to add new features, please feel free to submit an issue.
