

# train process

Update submodules:
```
git submodule init .
git submodule update
```

Train dataset
```
python3 train.py --img 640 --batch 32 --epochs 3 --data Grasshopper.yaml --weights yolo.pt --cache
```

For lower batch it will goes shorter while training but dataset can be contaminated.
```bash
python train.py --img 640 --batch 16 --epochs 3 --data coco128.yaml --weights grassgopper-best.pt --cache
```

After end of train we need to get best and last train files from `train/yolov5-for_train/runs/train/exp$s` path where $s is the latest exp numbered dir.

