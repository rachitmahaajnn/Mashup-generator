# Mashup-generator
# 🎵 YouTube Singer Mashup Generator

Create an automatic **audio mashup** of your favorite singer’s songs by downloading YouTube videos, trimming audio clips, and merging them into a single MP3 file.

---

## 📖 About The Project

The YouTube Singer Mashup Generator is a Python script that:

* Searches YouTube for a singer’s songs
* Downloads multiple videos automatically
* Extracts audio from each video
* Trims each audio clip to a fixed duration
* Merges all clips into one mashup file

It is useful for:

* Creating song mashups
* DJ practice clips
* College / mini projects
* Audio dataset preparation

---

## 🚀 Features

* 🎤 Search songs by singer name
* ⬇️ Auto download YouTube videos
* ✂️ Trim audio to fixed seconds
* 🔀 Merge multiple clips
* 🎧 Export final mashup as MP3
* 🖥️ Command-line based automation

---

## 🛠️ Tech Stack

* **Python 3**
* **yt-dlp** → Video downloading
* **pydub** → Audio processing
* **FFmpeg** → Audio conversion backend
* **OS / Sys** → File & argument handling

---

## 📂 Project Structure

```
youtube-mashup-generator/
│── downloads/        # Downloaded videos
│── mashup.py         # Main script
│── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/youtube-mashup-generator.git
cd youtube-mashup-generator
```

---

### 2️⃣ Install Dependencies

```bash
pip install yt-dlp pydub
```

---

### 3️⃣ Install FFmpeg

Pydub requires FFmpeg.

#### Windows:

Download from: [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html)
Add to system PATH.

#### Linux / Mac:

```bash
sudo apt install ffmpeg
# or
brew install ffmpeg
```

---

## ▶️ Usage

Run the script from terminal:

```bash
python mashup.py <SingerName> <NumberOfVideos> <AudioDuration> <OutputFileName>
```

---

### 📌 Arguments

| Argument       | Description                     |
| -------------- | ------------------------------- |
| SingerName     | Name of the singer              |
| NumberOfVideos | Videos to download (>10)        |
| AudioDuration  | Seconds to trim each clip (>20) |
| OutputFileName | Final mashup file name          |

---

### ✅ Example

```bash
python mashup.py "Arijit Singh" 15 30 arijit_mashup.mp3
```

This will:

* Download 15 Arijit Singh songs
* Trim 30 sec from each
* Merge into `arijit_mashup.mp3`

---

## 🔄 Workflow

1. Search YouTube → `ytsearch`
2. Download videos → `yt-dlp`
3. Convert to audio → `pydub`
4. Trim clips → Duration input
5. Merge all clips
6. Export final MP3

---

## ⚠️ Validations

The script enforces:

* Number of videos **> 10**
* Audio duration **> 20 sec**
* Integer input validation
* Error handling for file conversion

---

## 📦 Output

* Final mashup saved as **MP3**
* Stored in project root folder
* Downloaded videos stored in `/downloads`

---

## 🧑‍💻 Author

**Rachit Mahajan**
**102303495**
---

## 📜 License

This project is for **educational purposes only**.

Do not use downloaded content for commercial distribution without permission.

---

## ⭐ Support

If you like this project:

* Star ⭐ the repo
* Fork 🍴 it
* Share 📢 it

---
