set PATH=%PATH%;C:\\Software\\ffmpeg\\bin\\;C:\\Software\\ffmpeg\\lib\\;





\# Extract audio from a video file

ffmpeg -i input.mp4 -vn -acodec pcm\_s16le output.wav





\# Convert karaoke WAV to MP3

ffmpeg -i no\_vocals.wav -codec:a libmp3lame -qscale:a 2 karaoke.mp3



\# If you want it back as MP4 (audio-only track in an MP4 container)

ffmpeg -i no\_vocals.wav -c:a aac -b:a 192k karaoke.m4a

