# LLM-ASR
使用多模态大语言模型将音频转写为字幕文件

## 环境及依赖
### 环境
项目在Python 3.12.11环境下开发，使用时建议使用Conda虚拟环境
### 依赖
#### 0. uv
```
pip install uv
```
#### 1. torch
```
uv pip install torch==2.6.0 torchvision==0.21.0 torchaudio==2.6.0 --index-url https://download.pytorch.org/whl/cu126
```
#### 2. uvr
```
uv pip install git+https://github.com/RoadToNowhereX/ultimatevocalremover_api.git pyrubberband demucs
```
#### 3. transformers

Phi-4-multimodal-instruct建议使用transformers==4.51.3

Gemma-3n-E4B-it需要transformers>=4.53.0
```
uv pip install transformers
```
有部分LLM所需的依赖未出现在官方示例代码中，建议缺少部分自行安装
