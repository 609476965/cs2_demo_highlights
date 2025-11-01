## 使用说明 README OTHER LANGUAGE
[English](README/README.en.md) | [中文](README/README.zh.md)

# cs2_demo_highlights 🎥

> [!IMPORTANT]  
> 请使用 CS2 的无边框全屏模式，以便应用程序正常工作。
> 
> 这个应用只在 Windows 系统上运行！
> 
> 请确保正确设置 OBS。
>
> 目前无法录制名字中包含 Unicode 符号玩家的视频。
>
> 官匹录像可直接使用，**对于5E录像，需要按注释修改main.py**

## Installation

1. 安装 Python （版本 >= 3.11）
2. 下载这个仓库
3. 打开一个 cmd / powershell
4. `pip install -r requirements.txt`
5. 调整 config.py（如有需要，调整 CS2 加载和演示加载时间）

## OBS Setup

1. 创建一个新配置文件，命名为cs2_demo_highlights
2. 设置你的 OBS 编码器、分辨率、帧率等
3. 为 cs2 添加一个窗口捕获源，**禁用光标捕获**
4. 启用 WebSocket：工具 > WebSocket 服务器设置 > 启用它，设置密码
5. 更新 config.py 文件，加入你的 WebSocket 密码和端口

## Usage
1. 在解压下载归档文件的文件夹中打开 cmd / PowerShell 窗口。
2. 将你的比赛录像文件放在 main.py 文件所在的同一个文件夹中
3. 打开CS2游戏到主界面
4. run `python main.py`
5. 浏览提示信息
6. 等待 CS2 启动，并在进程结束之前（与比赛录像播放器断开连接）不要进行任何操作

## Credits
本代码使用了以下库：
- [PyGetWindow](https://github.com/asweigart/PyGetWindow)
- [PyAutoGUI](https://github.com/asweigart/pyautogui)
- [pick](https://github.com/aisk/pick)
- [obs-websocket-py](https://github.com/Elektordi/obs-websocket-py)
- [moviepy](https://github.com/Zulko/moviepy)
- [demoparser2](github.com/LaihoE/demoparser)

## Contributing
修改自https://github.com/MarcelDev/cs2_demo_highlights
