# How to config
```shell
pip install openai-whisper
pip install ffmpeg-python
pip install zhconv
pip install imageio
pip install imageio[ffmpeg]
```

# How to use
```
python main.py "C:\Users\Administrator\Downloads\1.mp4" "Chinese" "C:\Users\Administrator\Downloads\1.srt"
```
Parameter description:
1. Input video file
2. Input video language
3. Output srt subtitle file path

# Note
The first time the program runs it may take some time.<br>

If you are a Chinese user, you need a VPN during initialization, otherwise the network is unstable.<br>

This project is based on the blog "https://blog.csdn.net/weixin_48169169/article/details/134998361" adapted and summarized<br>

Non-commercial use and secondary creation are allowed<br>
