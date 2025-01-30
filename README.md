# comfyui_flow
用来保存我使用的一些comfyui相关的东西

## 工作流列表
fastpaint   快速修复（视频去固定位置水印）

## 讨饭
以下是我的USDT钱包，我很可爱，请给我钱 (╹ڡ╹ )
```
TRNVdKwdMZgbGtWyxBao8gRcKN2tf9aBHv
```
## 安装
### Liunx 安装GPU驱动 
```bash
curl -fSsL -O https://github.com/GoogleCloudPlatform/compute-gpu-installation/releases/download/cuda-installer-v1.1.0/cuda_installer.pyz
#安装驱动
#python3 cuda_installer.pyz install_driver
#安装cuda
python3 cuda_installer.pyz install_cuda
#验证cuda
python3 cuda_installer.pyz verify_cuda
#验证驱动
nvidia-smi
```
### 安装UV管理环境
```bash
#安装uv
curl -LsSf https://astral.sh/uv/install.sh | sh
source $HOME/.local/bin/env
```
### 安装comfyui 使用3.10版本
#### 下载comfyui
```bash
git clone https://github.com/comfyanonymous/ComfyUI.git 
cd ComfyUI
```
#### 设置python环境
```
#虚拟环境
uv venv -p 3.10
source .venv/bin/activate

# 安装必备包
uv pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu121
uv pip install -r requirements.txt
uv pip install pip

# 将虚拟环境写入到bashrc每次登录就能用
# echo 'source $(pwd)/.venv/bin/activate' >> ~/.bashrc && source ~/.bashrc

```
