# MP3 Toolkit

A collection of Python command-line utilities for audio conversion and YouTube media operations.

## Features

* **MP4 to MP3** — Extract audio from local MP4 files.
* **YouTube Searcher** — Search YouTube videos using the YouTube Data API v3.
* **YouTube to MP3** — Extract audio from YouTube URLs using yt-dlp.

## Project Structure

```text
MP3/
├── converter_mp4/
│   └── main.py
├── youtube-searcher/
│   └── main.py
└── yt-dlp/
    └── main.py
```

## Requirements

* Python 3.9+
* FFmpeg
* YouTube Data API v3 key (for YouTube Searcher)

Install dependencies:

```bash
pip install moviepy requests yt-dlp
```

## Usage

### MP4 to MP3

```bash
python converter_mp4/main.py
```

Enter the input MP4 file path and desired MP3 output name.

### YouTube Searcher

```bash
python youtube-searcher/main.py
```

Currently searches for `space exploration` and displays up to five video results.

Requires a valid YouTube Data API key.

### YouTube to MP3

```bash
python yt-dlp/main.py
```

Enter a YouTube URL when prompted.

The script extracts the best available audio and converts it to MP3 at 192 kbps.

## Notes

* Each utility operates independently.
* Output files are saved in the current working directory.
* FFmpeg must be installed and accessible through PATH.
* Use only media you own or are authorized to download.
* Respect copyright laws and platform terms.

## License

No license has been specified yet.
