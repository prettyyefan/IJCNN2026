
# 激活虚拟环境
.\venv\Scripts\activate 

python visualize_debug.py

# 上传github仓库步骤
# first
git init

git add memo.md

git commit -m "first commit code"

git branch -M main

git remote add origin https://github.com/prettyyefan/IJCNN2026.git

git pull origin main --allow-unrelated-histories

# after

git add memo.md

git commit -m "update 2025.12.14"

git push -u origin main

# 硬件信息
    Python版本：Python 3.10.11
    CUDA版本：（nvidia-smi）CUDA Version: 12.2
    PyTorch版本：2.5.1+cu121
    TorchVision版本： 0.20.1+cu121

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

# 训练代码
yolo detect train model=yolov8n.pt data=data.yaml epochs=10 imgsz=640 device=0 batch=8 amp=False

# 备注（yolo的记忆功能，记得删除不好的，非必要的记忆）
C:\Users\yefan\Desktop\yefan\IJCNN\datasets\cityscapes\labels\

train.cache
val.cache