ComfyUI
=======
The most powerful and modular stable diffusion GUI and backend.
-----------
![ComfyUI Screenshot](comfyui_screenshot.png)

This ui will let you design and execute advanced stable diffusion pipelines using a graph/nodes/flowchart based interface. For some workflow examples and see what ComfyUI can do you can check out:
### [ComfyUI Examples](https://comfyanonymous.github.io/ComfyUI_examples/)

### [Installing ComfyUI](#installing)

### run
1. 安装环境
```shell
cd ComfyUI

python3 -m venv venv

ls

source venv/bin/activate

deactivate
```
2. 下载训练模型
https://huggingface.co/stabilityai/sdxl-turbo/tree/main
> eg: 下载sd_xl_turbo_1.0_fp16.safetensors模型，并将其放在/models/checkpoints文件夹下面

3. 安装comfyui manager
```shell
cd custom_nodes
git clone https://github.com/ltdrdata/ComfyUI-Manager
```

4. 安装python依赖
```shell
cd .. # 定位到ComfyUI文件夹
pip install -r requirements.txt
```

5. 加载模型并启动
```shell
python main.py --force-fp16
```

6. 打开右侧面板
快捷键 cmd + 0


7. 使用默认工作流，text2img模型，点击Queue Prompt 生成图片