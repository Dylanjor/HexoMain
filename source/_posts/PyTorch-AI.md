---
title: PyTorch-AI
date: 2025-10-24 15:43:24
tags: AI
category: AI
index_img: /img/16e97308c2e942a28c68afb22a36023b.jpg
banner_img: /img/94a43dbbc6ee402897d7996560db98e5.jpg
---

## PyTorch-AI


### WINDOWS 下载安装PyTorch
pip 安装

(首先要有Python环境)
```
# 首先访问 Python官网 https://www.python.org/downloads/
# 或者使用命令行工具下载（需要 curl 或 wget）
curl -o python-installer.exe https://www.python.org/ftp/python/3.11.4/python-3.11.4-amd64.exe 
python-installer.exe /quiet InstallAllUsers=1 PrependPath=1
```

```
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu126 
```

Windows长路径支持
```
reg add HKLM\SYSTEM\CurrentControlSet\Control\FileSystem /v LongPathsEnabled /t REG_DWORD /d 1

pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
```

```
import torch
x = torch.rand(5, 3)
print(x)
```