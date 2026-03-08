# JM-NcatBot

基于 Napcat, NcatBot, JMComic-Crawler-Python 的 QQ 机器人。

## Install

1. 克隆项目

```bash
git clone https://github.com/Sora-o-tobu/JM-NcatBot.git
cd JM-NcatBot
```

2. 安装依赖 

```bash
pip install -r requirements.txt`
```

3. 下载 napcat

通过 NapCatQQ-Desktop.exe，选择“我是老手”，然后在组件中进行安装。安装完成后，请将 runtime/NapCatQQ 文件夹移动至根目录并命名为 napcat。

> https://github.com/NapNeko/NapCatQQ-Desktop/releases/tag/v1.7.28

4. 运行

对于 Windows，通过 napcat 文件夹下的 `launcher.bat` 启动 Napcat，进入 webui（一般为 `localhost:6099`），添加 websocket Server，host 和 port 选择 `ws://localhost:3001`。

Linux 用户自行查阅 napcat 官方文档，换用合适的 napcat 文件。

更改 `main.py` 各参数，运行 `python main.py`，接下来按照指示操作。

具体操作以及参数作用可参照 Reference 官方文档。

## Usage

输入 /jm <id:xxx> ，机器人会自动下载生成 pdf 并发送消息。

例： /jm 350234

## Reference

- [NapCatQQ](https://napcat.napneko.icu/)
- [NcatBot](https://docs.ncatbot.xyz/)
- [JMComic-Crawler-Python](https://github.com/hect0x7/JMComic-Crawler-Python)