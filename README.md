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

经过多次修改稍微复杂点的防撤回插件

-> 更新后可能要删掉bot目录下\data\enablelist 文件夹内的配置文件,并重新设置

开启后群内撤回消息会被bot发送

群主可以开关本群的防撤回

不建议使用私聊功能,容易风控(建议收购企鹅🐧)

超级用户可以开启一个群,每次有撤回消息会在群内通知,这样不用多次私聊转发,群内消息减小企鹅风控

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
| 开启/关闭绕过管理层 |管理员/群主不会被防撤回,仅限群内 |
| 防撤回菜单 |打开本插件菜单 |
| 开启/关闭防撤回私聊gid uid |超级管理员私聊使用,gid群号的群撤回消息会私聊给uid的用户,如果群没开启防撤回就不生效 |
| 查看防撤回私聊 |查看私聊列表,私聊使用,会返回json数据.|
| 开启防撤回私聊 gid |设置防撤回触发后监听的群,一个参数群号(ps.仅限一个群[建议是一个私人小群专门用来干这事]重新设置会覆盖)|
| 关闭防撤回私聊 |无参数,删除这个监听群,不监听 |
| 查看防撤回监听 |查看监听的群和发送的群,一个json |
| 添加/删除防撤回监听 gid|添加防撤回被监听的群,一次一个[不建议太多,会风控]|

Tips防撤回的英文指令 : enable/disable, enable/disable here, bypass/no bypass here, clear list, antirecall menu, enable/disable private msg, enable/disable/add/remove/view listener, list private msg
