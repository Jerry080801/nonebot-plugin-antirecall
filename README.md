<div align="center">
  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
  <br>
  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
</div>

<div align="center">

# nonebot-plugin-antirecall

_✨ NoneBot 防撤回插件 ✨_


<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/A-kirami/nonebot-plugin-namelist.svg" alt="license">
</a>
<a href="https://pypi.python.org/pypi/nonebot-plugin-namelist">
    <img src="https://img.shields.io/pypi/v/nonebot-plugin-namelist.svg" alt="pypi">
</a>
<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">

</div>


## 📖 介绍

简单的防撤回插件

开启后群内撤回消息会被bot发送

群主可以开关本群的防撤回

超级用户可以查看全局防撤回和列表。

## 💿 安装

<details>
<summary>使用 nb-cli 安装</summary>
在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装

    nb plugin install nonebot-plugin-antirecall

</details>

<details>
<summary>使用包管理器安装</summary>
在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

<details>
<summary>pip</summary>

    pip install nonebot-plugin-antirecall
</details>
<details>
<summary>pdm</summary>

    pdm add nonebot-plugin-antirecall
</details>
<details>
<summary>poetry</summary>

    poetry add nonebot-plugin-antirecall
</details>
<details>
<summary>conda</summary>

    conda install nonebot-plugin-antirecall
</details>

打开 nonebot2 项目的 `bot.py` 文件, 在其中写入

    nonebot.load_plugin('nonebot_plugin_antirecall')

</details>


## 🎉 使用
### 指令表
| 指令 | 说明 |
|:-----:|:----:|
| 开启/添加防撤回, enable + 群号1 群号2 ...|开启群的防撤回 |
| 关闭/删除防撤回, disable + 群号1 群号2 ...|关闭群的防撤回 |
| 查看防撤回群聊 |查看防撤回群聊 |
| 防撤回菜单 |打开本插件菜单 |
