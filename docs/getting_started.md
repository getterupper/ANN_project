# Prerequisites

**Please ensure you have prepared the environment and the SemanticKITTI dataset.**

# Train and Test

Train our model with temporal information with 4 GPUs
```
./tools/dist_train.sh ./projects/configs/voxformer/VoxFormer-S.py 4
```
```
./tools/dist_train.sh ./projects/configs/voxformer/VoxFormer-T.py 4
```

Eval our model with temporal information with 4 GPUs
```
./tools/dist_test.sh ./projects/configs/voxformer/VoxFormer-S.py ./path/to/ckpts.pth 4
```

```
./tools/dist_test.sh ./projects/configs/voxformer/VoxFormer-T.py ./path/to/ckpts.pth 4
```