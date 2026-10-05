# NETFO Car Studio — model files

Model files that NETFO Car Studio downloads on first use. No app code is kept here.

## AI windows (Windows, NVIDIA graphics) — release `aiwindows-model-1`

Stable Diffusion v1.5 inpainting
([stable-diffusion-v1-5/stable-diffusion-inpainting](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-inpainting),
revision `8a4288a76071f7280aedbdb3253bdb9e9d5d84bb`), exported to ONNX for ONNX Runtime + DirectML:

| File | What |
|---|---|
| `unet_fp16.onnx` | UNet, fp16 |
| `vae_encoder.onnx`, `vae_decoder.onnx` | VAE, fp32 (scaling factor built in) |
| `embeds.npy` | the app's fixed prompt / negative prompt, already encoded |
| `SHA256SUMS` | checksums (the app verifies every file) |

The weights are unchanged apart from the format conversion. They are covered by the
**CreativeML Open RAIL-M** licence in [LICENSE](LICENSE), including its use restrictions (Attachment A).
