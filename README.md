# Revisiting Graph Contrastive Learning on Anomaly Detection from a Structural Imbalance Perspective

## Code structure
| *folder*  |                         description                          |
| :-------: | :----------------------------------------------------------: |
|   Data    |      Datasets.       |
|   AD-GCL    | AD-GCL implementation code is provided. |

## Datasets

| **Dataset** |  # Nodes  |  # Edges  |  # Attribute  |  # Anomalies  |
| :---------: | :--------: | :-----: | :--------: | :--------: |
|  **Bitcoinotc**   |  5,881  |  35,592  |  128  |  300  |
|  **BITotc**   |  4,863  |  28,473  |  128  |  300  |
| **BITalpha** |  3,219  |  19,364  |  128  |  300  |


## Usage
```python
# Bitcoinotc
python ./AD-GCL/run.py --dataset 'bitcoinotc' --lr 4e-4 --num_epoch 100 --threshold 8 --gpu_id 0

# BITotc
python ./AD-GCL/run.py --dataset 'bitotc' --lr 5e-4 --num_epoch 100 --threshold 7 --gpu_id 0

# BITalpha
python ./AD-GCL/run.py --dataset 'bitalpha' --lr 5e-3 --num_epoch 100 --threshold 8 --gpu_id 0
```


## Dependencies

- Python 3.8.13
- PyTorch 1.12.1
- dgl 0.4.3.post1
- Scipy 1.9.1
- Tqdm 4.64.1
