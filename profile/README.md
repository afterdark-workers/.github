# afterdark-workers

Ready-to-build [RunPod Serverless](https://runpod.io?ref=qpguwapm) workers for 18+ image and video models from Civitai and Hugging Face. Each repo is a template: make a private copy, paste your Civitai token (Hugging Face ones need none), point a RunPod endpoint at it. The model is baked into the image and checked by SHA-256 at build time.

**[Docs](https://afterdark-workers.github.io/)** ([source](https://github.com/afterdark-workers/afterdark-workers.github.io)) — every model, the GPU it needs, and how to run it on RunPod or Modal.

No RunPod account yet? [Sign up here](https://runpod.io?ref=qpguwapm) — a referral link: after you first add $10, RunPod gives you a bonus credit (usually $5–10).

### Photoreal

| Model | Base | Engine | Repo |
|---|---|---|---|
| Krea 2 DirtyUncut | Krea 2 | ComfyUI | [krea2-dirtyuncut](https://github.com/afterdark-workers/krea2-dirtyuncut) |
| Krea 2 FinePorn | Krea 2 | ComfyUI | [krea2-fineporn](https://github.com/afterdark-workers/krea2-fineporn) |
| Lustify SDXL | SDXL | ComfyUI | [lustify-sdxl](https://github.com/afterdark-workers/lustify-sdxl) |
| Fluxmania Kreamania | FLUX.1 dev | ComfyUI | [fluxmania](https://github.com/afterdark-workers/fluxmania) |
| Z-Image CyberRealistic | Z-Image | ComfyUI | [zimage-cyberrealistic](https://github.com/afterdark-workers/zimage-cyberrealistic) |
| Z-Image IntoRealism | Z-Image | ComfyUI | [zimage-intorealism](https://github.com/afterdark-workers/zimage-intorealism) |
| Z-Image BigLove | Z-Image | ComfyUI | [zimage-biglove](https://github.com/afterdark-workers/zimage-biglove) |
| PornMaster Z-Image Turbo | Z-Image | ComfyUI | [pornmaster-zimage](https://github.com/afterdark-workers/pornmaster-zimage) |
| Z-Image Asian Utopian | Z-Image | ComfyUI | [zimage-asianutopian](https://github.com/afterdark-workers/zimage-asianutopian) |
| Z-Image Nina | Z-Image | ComfyUI | [zimage-nina](https://github.com/afterdark-workers/zimage-nina) |
| NoctQ V4 | Qwen-Image 2.1 | ComfyUI | [noctq](https://github.com/afterdark-workers/noctq) |
| Chroma1-HD | Chroma | ComfyUI | [chroma1-hd](https://github.com/afterdark-workers/chroma1-hd) |
| Chroma1-Flash | Chroma | ComfyUI | [chroma1-flash](https://github.com/afterdark-workers/chroma1-flash) |
| Chroma1-Base | Chroma | ComfyUI | [chroma1-base](https://github.com/afterdark-workers/chroma1-base) |
| SPARK.Chroma v1 | Chroma | ComfyUI | [spark-chroma](https://github.com/afterdark-workers/spark-chroma) |
| CyberRealistic Pony | Pony (SDXL) | AUTOMATIC1111 | [a1111-cyberrealistic-pony](https://github.com/afterdark-workers/a1111-cyberrealistic-pony) |

### Anime · cartoon

| Model | Base | Engine | Repo |
|---|---|---|---|
| Pony Diffusion V6 XL | Pony (SDXL) | ComfyUI | [pony-v6-xl](https://github.com/afterdark-workers/pony-v6-xl) |
| WAI-Illustrious-SDXL | Illustrious (SDXL) | ComfyUI | [wai-illustrious-sdxl](https://github.com/afterdark-workers/wai-illustrious-sdxl) |
| Pony Diffusion V6 XL | Pony (SDXL) | AUTOMATIC1111 | [a1111-pony-v6-xl](https://github.com/afterdark-workers/a1111-pony-v6-xl) |

### Edit a picture

| Model | Base | Engine | Repo |
|---|---|---|---|
| Qwen-Image-Edit Rapid AIO | Qwen-Image-Edit | ComfyUI | [qwen-edit-rapid-aio](https://github.com/afterdark-workers/qwen-edit-rapid-aio) |

### Picture to video

| Model | Base | Engine | Repo |
|---|---|---|---|
| Wan 2.2 Enhanced NSFW 14B | Wan 2.2 | ComfyUI | [wan22-enhanced-nsfw](https://github.com/afterdark-workers/wan22-enhanced-nsfw) |

Two engines — they work the same from Cobalt Pear:

- **ComfyUI** — a node workflow; every step can be tuned. Takes API-format workflows (based on [`runpod/worker-comfyui`](https://github.com/runpod-workers/worker-comfyui)).
- **AUTOMATIC1111** — a few settings and done (prompt, steps, sampler …), the same as AUTOMATIC1111's own API. It runs without its web page.

Every repo has a `pack.json`, so [Cobalt Pear](https://cobaltpear.github.io/) — a one-page web app — can drive it: add the repo URL, your endpoint ID and API key, then just type. [Try the demo](https://cobaltpear.github.io/demo/) without RunPod.

You download each model yourself (Civitai models with your own account) and are responsible for following its license.
