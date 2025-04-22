# 🎞️ GIF to MP4 Converter

**A simple script to convert GIF files into optimized MP4 videos.**  
Built for speed, simplicity, and batch automation.

---

## 💡 Why This Exists

GIFs are fun, but not very efficient. This tool helps you quickly convert them into modern MP4 files — smaller in size, better in quality, and ready for social media or the web.

---

## 🛠️ Features

- ✅ Converts single or multiple `.gif` files
- ✅ CLI-based (no GUI needed)
- ✅ Optimized for file size using `ffmpeg`
- ✅ Easy to extend or embed in other tools

---

## ⚙️ How It Works

This script uses [FFmpeg](https://ffmpeg.org/) under the hood:

```bash
ffmpeg -i input.gif -movflags faststart -pix_fmt yuv420p -vf "scale=trunc(iw/2)*2:trunc(ih/2)*2" output.mp4
