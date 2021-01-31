# useful_ffmpeg_scripts


```
# 升半音
ffmpeg -i "心灵之约.mp3" -filter_complex "asetrate=48000*2^(1/12),atempo=1/2^(1/12)" "output.mkv"
 
# 升全音
ffmpeg -i "心灵之约.mp3" -filter_complex "asetrate=48000*2^(2/12),atempo=1/2^(2/12)" "output.mkv"
 
# 降半音
ffmpeg -i "心灵之约.mp3" -filter_complex "asetrate=48000*2^(-1/12),atempo=1/2^(-1/12)" "output.mkv"
 
# 降全音
ffmpeg -i "心灵之约.mp3" -filter_complex "asetrate=48000*2^(-2/12),atempo=1/2^(-2/12)" "output.mkv"
```

如果不需要保持原速，就删掉atempo
