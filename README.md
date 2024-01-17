# Youtube Scripts

A collection of youtube scripts I cobbled together

# Usage

`[script name] [URL]`

# youtube

Downloads a youtube video from the provided url with the best resolution into a temporary file and calls mpv. I created this script as a shorthand to get around the youtube anti-adblock nonsense.

# ystream

I experienced buffering even when calling `mpv [URL]`, so that wasn't enough to get around youtube nonsense, so I created the previous script. Turns out, the video plays fine if I pipe the output of `yt-dlp` into `mpv`. One downside is, since I want to use the best resolution, yt-dlp has to combine the audio and video files with ffmpeg, so seeking to a specific point in the video is impossible.

# ydl

I created this to download a youtube video to the current directory with aria2.
