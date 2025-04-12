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

After running the program, the following may occur:<br>
```
F:\python\project\srt_geter(根据视频生成srt)>python main.py F:\DisAssembly\study\video\RE_06.mp4 Chinese F:\DisAssembly\study\video\RE_06.srt
C:\Users\Administrator\AppData\Local\Programs\Python\Python38\lib\site-packages\whisper\__init__.py:150: FutureWarning: You are using `torch.load` with `weights_only=False` (the current default value), which uses the default pickle module implicitly. It is possible to construct malicious pickle data which will execute arbitrary code during unpickling (See https://github.com/pytorch/pytorch/blob/main/SECURITY.md#untrusted-models for more details). In a future release, the default value for `weights_only` will be flipped to `True`. This limits the functions that could be executed during unpickling. Arbitrary objects will no longer be allowed to be loaded via this mode unless they are explicitly allowlisted by the user via `torch.serialization.add_safe_globals`. We recommend you start setting `weights_only=True` for any use case where you don't have full control of the loaded file. Please open an issue on GitHub for any issues related to this experimental feature.
  checkpoint = torch.load(fp, map_location=device)
正在识别：study\video\RE_06.mp4 --2025-04-12 12:38:21
视频时长：01:02:08,780
```
Don't worry about the error message, it is already working.<br>

This project is based on the blog "https://blog.csdn.net/weixin_48169169/article/details/134998361" adapted and summarized<br>

Non-commercial use and secondary creation are allowed<br>
