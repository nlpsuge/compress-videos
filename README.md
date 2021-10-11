# compress-videos
Compress all videos under the current folder recursively.

# Usage

## Compress videos whose size are bigger than N
- Compress videos whose size are bigger than 500M
```Bash
compress-videos -size +500M
```
- Compress videos whose size are bigger than 1G
```Bash
compress-videos -size +1G
```
- Compress all videos
```Bash
compress-videos -size +0M
```

## Answer `No` to all questions produced by `ffmpeg` during processing videos
```Bash
echo N | compress-videos -size +0M
```

I suggest give `No` to all questions. If `ffmpeg` find out that a video has been processed, it will throw a question at you to ask if you want to overwrite the exsting compressed video.
