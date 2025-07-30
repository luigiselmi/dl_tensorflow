Experiments
===========
In this document are reported the results of the experiments with Deep Learning algorithms. The RAM represents the average memory used to run the notebook. The GPU RAM represent the GPU memory used, mainly to fit the model, and the memory available. The validation loss and the accuracy are the best results during the training.

| Notebook | Task | Model | DL platform | Date | Exp. number | Optimizer | Learning rate | Loss function | Batch size | Num. epochs | Time per epoch (s)| Augmentation (% data increase)| Best validation loss | Best accuracy | RAM (GB) | GPU type | RAM GPU |  
|:--------|:--------|:------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|:---------|
| [Rooftop segmentation v3](rooftops_segmentation_v3.ipynb) | Semantic segmentation | U-Net Xception | Colab Tensorflow | 2025-07-28| 1 | Adam | 10^-4 | sparse categorical crossentropy | 4 | 40 | 80 | No | 0.2718 | 0.9178 | 9.5 | Nvidia T4 | 3.2 / 15.0 |
| [Rooftop segmentation v3](rooftops_segmentation_v3.ipynb) | Semantic segmentation | U-Net Xception | Colab Tensorflow | 2025-07-30| 1 | Adam | 10^-4 | sparse categorical crossentropy | 4 | 40 | 80 | Yes (500%) | 0.3736 | 0.9216 | 4.4 | Nvidia L4 | 3.2 / 22.5 |
| [Advanced Computer Vision v2](advanced_computer_vision_v2.ipynb) | Semantic segmentation | Encoder-Decoder | Colab Tensorflow | 2025-07-29| 1 | Adam | 10^-3 | sparse categorical crossentropy | 64 | 40 | 80 | No | 0.3712 | 0.8599 | 9.5 | Nvidia T4 | 13.7 / 15.0 | 
| [Advanced Computer Vision v2](advanced_computer_vision_v2.ipynb) | Semantic segmentation | Encoder-Decoder | Colab Tensorflow | 2025-07-29| 2 | Adam | 10^-3 | sparse categorical crossentropy | 64 | 40 | 6 | Yes (400%) | 0.3916 | 0.8508 | 10.8 | Nvidia A100 | 16.50 / 40.0 | 

