# ComfyUI-LoRA


# ComfyUI-3D
### Links
[![ComfyUI](https://img.shields.io/badge/ComfyUI-GitHub-orange?logo=github)](https://github.com/comfyanonymous/ComfyUI)
[![ComfyUImanager](https://img.shields.io/badge/ComfyUImanager-GitHub-green?logo=github)](https://github.com/ltdrdata/ComfyUI-Manager)
[![Badge hunyuan3DWrapper](https://img.shields.io/badge/Hunyunan3DWrapper-GitHub-blue?logo=github)](https://github.com/kijai/ComfyUI-Hunyuan3DWrapper)

Este repositório mostra como utilizar o modelo **Hunyuan 3D** no **ComfyUI** para transformar uma **imagem 2D em um modelo 3D texturizado** de forma simples e visual.

### Requisitos
- ComfyUI
- Python 3.10+
- GPU com suporte a CUDA (recomendado)

### Instalação para gerar 3D
1. Abre custom_node dentro do diretório de ComfyUI:
   ```bash
   cd custom_nodes
3. Instalar Hunyuan 3D Wrapper:
   ```bash
   git clone https://github.com/kijai/ComfyUI-Hunyuan3DWrapper.git
   cd ComfyUI-Hunyuan3DWrapper
   pip install -r requirements.txt
5. Instalar custom rasterizer (pytorch e CUDA precisa ser compatível):
   ```bash
   cd hy3dgen/texgen/custom_rasterizer
   pip install .
7. Instalar o modelo [hunyuan3d-div-v2-0-fp16.safetensors](https://huggingface.co/Kijai/Hunyuan3D-2_safetensors/tree/main) dentro do `ComfyUI/models/diffusion_models`.
8. Dentro do ConfyUI instala o custom node [Essentials](https://github.com/cubiq/ComfyUI_essentials.git), se tiver Manager instala através do **Install Missing Custom Nodes**.

### Workflow para gerar 3D
[Clique aqui para ver o workflow](./Hunyuan3D-CG.json)

### Exemplo de etapas para gerar 3D
![input](imagens/processo.png)
