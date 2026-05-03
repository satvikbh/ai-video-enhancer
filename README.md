# 🎬 AI Video Enhancer — Free Video Upscaling with Real-ESRGAN

Upscale any video to **2K (2560×1440)** using AI — completely free on Google Colab.

No signups. No watermarks. No limits. Just a single Jupyter notebook.

## 🚀 Quick Start

1. Open the notebook in Google Colab
2. Set runtime to **T4 GPU** (`Runtime → Change runtime type → T4 GPU`)
3. Run all cells top to bottom
4. Upload your video → get the enhanced version


## 📊 Results

| | Before | After |
|---|---|---|
| Resolution | 810×454 | 2560×1440 |
| Bitrate | 96 kbps | 600+ kbps |
| Text clarity | Blurry, unreadable | Sharp, crystal clear |
| Cost | — | ₹0 |

## ⚙️ How It Works

The pipeline is simple:

1. **Extract** — FFmpeg extracts every frame from the video
2. **Upscale** — Real-ESRGAN (AI model) upscales each frame 2× on a T4 GPU
3. **Sharpen** — Subtle unsharp mask for extra clarity
4. **Reassemble** — FFmpeg combines upscaled frames + original audio into the final video

The output is a standard H.264 MP4 (yuv420p, High profile) that plays everywhere — Windows, Mac, phones, browsers.

## 🛠️ Tech Stack

- **Real-ESRGAN** — State-of-the-art AI upscaling model (open-source)
- **FFmpeg** — Video frame extraction and reassembly
- **Google Colab** — Free T4 GPU for inference
- **Python** — Pipeline orchestration

## 📝 Notes

- Works best with videos up to 5 minutes (Colab session limits)
- GPU-intensive — each frame takes ~0.3s on T4
- Audio is preserved from the original video
- Output is H.264 High Profile — compatible with all players

## 📄 License

MIT — use it however you want.

## ⭐ Star This Repo

If this saved you from paying for a video enhancer tool, drop a star. It helps others find it too.
