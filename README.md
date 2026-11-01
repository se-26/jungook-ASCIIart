<div align="center">

# 🐰💜 ASCII Video Art

**every frame of a video, rebuilt out of letters and symbols instead of pixels**

### ▶️ [Watch the live demo](https://shraaaa17.github.io/jungook-ASCIIart/)

</div>

---

### ✨ what is this?
A small coding art project that turns **any video** into ASCII art.
Give it a video, and it converts each frame into characters, so the
whole clip plays back as moving text.

I first made it for a Jungkook edit 💜, but it isn't limited to that.
**You can import any video of your own and convert it.**

### 🎬 how it works
1. 🎞️ the video is read frame by frame
2. 🌗 each frame is turned into grayscale (light and dark values)
3. 🔤 every small block of pixels is replaced with a character:
   dark areas get denser characters, light areas get sparser ones
4. 🖥️ the characters are put back together as frames and played as a video

### 🛠️ built with
- Python
- [OpenCV](https://opencv.org/) for reading and writing video frames
- [NumPy](https://numpy.org/) for the per-frame math
- [Pillow](https://python-pillow.org/) for rendering the character glyphs
- [FFmpeg](https://ffmpeg.org/) (optional) to re-encode the final MP4 with audio

### 🚀 how to use

```bash
# 1. clone this repo
git clone https://github.com/shraaaa17/jungook-ASCIIart.git
cd jungook-ASCIIart

# 2. install the dependencies
pip install opencv-python numpy pillow

# 3. add your video as input.mp4 and run
python main.py
```

The script writes `ascii_hacker_animation.mp4` and then plays it in a
window. Press **Space** to pause/resume, **Q** or **Esc** to close it.

If `ffmpeg` is installed, the final MP4 keeps the original audio;
otherwise the silent intermediate `ascii_video_silent.mp4` is used.

### 🎛️ settings you can change
- `ASCII_CHARS` — which letters and symbols are used
- `MAX_COLUMNS`, `CELL_WIDTH`, `CELL_HEIGHT` — character grid density
- `CYAN_TINT`, `GLOW_STRENGTH`, `GLOW_BLUR` — colour and glow

### 📸 preview
The generated animation is published on the
[live demo page](https://shraaaa17.github.io/jungook-ASCIIart/).

### 📝 note
This is a fan-made art project, made for learning and fun.
Videos you convert belong to their original owners, so only use
videos you have the right to use.

---

<div align="center">

*made with 💜 by [Shravani](https://www.instagram.com/shraisqt)*

</div>
