# StableDiffusion
直接运行，一条命令：
注意需要 ~140G 存储空间
```bash
docker run -it \
  --restart=always \
  --name comfyui \
  --gpus '"device=0"' \
  -p 8188:8188 \
  pinetrick/comfyui:withmodelnew \
 /bin/bash -c "source /root/ComfyUI/venv/bin/activate && cd /root/ComfyUI/ && python3 main.py --listen 0.0.0.0 & exec bash"
```
