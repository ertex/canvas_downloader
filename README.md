# canvas_downloader
This script is to download very specific files from chalmers . instructure
More specificly videostreams, like lectures then convert them to a MP4 format using FFMPEG.

Usage

Find a videostream using inspect element on canvas and looking at the transmitted packages.
While watching a video 'large' (1Mb) files are being downloaded in a .ts format, these are short videoclips.
Copy the URL of one of them. it should look something like this ....../name/a.mp4/seg-3-v1-a1.ts

then use the script ./downloader [INSERT URL HERE] and watch it go.

Bugs

the number behind "seg-" at then end must be a single digit because RegEX didn't behave and I could not be bothered. 
