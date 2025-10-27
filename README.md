# Audio Stem Separation & Key/BPM Detection (Demucs + Essentia)

This Colab notebook separates any uploaded song into individual stems (vocals, drums, bass, etc.) using **[Demucs](https://github.com/facebookresearch/demucs)** and then analyzes its **key** and **BPM** with **[Essentia](https://essentia.upf.edu/)**.  
It’s a simple, all-in-one tool for musicians, producers, and remixers who want to explore a track’s structure or create custom backing stems.

---

## Features
- **Automatic stem splitting** via Demucs (4-stem or 6-stem model)
- **Key and BPM detection** powered by Essentia’s high-quality audio analysis
- **FFmpeg integration** for universal audio format support (MP3, WAV, FLAC, etc.)
- **One-click ZIP export** of separated stems for easy download
- Works entirely in **Google Colab** — no local installation needed

---

## Usage
1. Open the notebook in Google Colab.  
2. Run the first cell to install dependencies:
   ```bash
   !pip -q install demucs essentia ffmpeg-python
   !apt-get -qq update && apt-get -qq install -y ffmpeg
