# Few-shot Point Cloud Semantic Segmentation via Support-Query Feature Interaction

## Installation
This repository is tested with `python 3.7.17`, `torch 1.7.0+cu110`
```
pip install tensorboard h5py transforms3d tqdm scipy faiss-cpu torch_cluster
```

## Data preparation
Follow [attMPTI](https://github.com/Na-Z/attMPTI)

## Running 
#### Training
First, pretrain the segmentor which includes feature extractor module on the available training set:

    bash pretrain.sh

Second, train our method:
	
	bash train.sh


#### Evaluation
    
    bash eval.sh

Note that the above scripts are used for 2-way 1-shot on ScanNet (S^0). You can modified the corresponding hyperparameters to conduct experiments on other settings. 


## Acknowledgement
We thank [DGCNN (pytorch)](https://github.com/WangYueFt/dgcnn/tree/master/pytorch), [attMPTI](https://github.com/Na-Z/attMPTI) for sharing their source code.
