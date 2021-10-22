# How to make train

Into this directory:

```
git submodule init .
git submodule update
python3 train.py --img 640 --batch 32 --epochs 3 --data Grasshopper.yaml --weights yolo.pt --cache
```