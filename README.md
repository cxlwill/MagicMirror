# Magic Mirror
基于树莓派的自制魔镜，集成 Magic Mirror，Google Assistant，Home assistant，Homebridge及中文聊天机器人。

实现功能：

- 人机语音交互，包括语音控制智能家居设备、日常聊天等
- 动态可触控房屋平面图
- 摄像头实时监控
- 基本的人脸识别功能

欢迎加入项目 [Slack](https://join.slack.com/t/magicmirror-cn/shared_invite/MjExNjg5MzY0NTQ1LTE0OTk5MzQyNjktMjc5YjNmMjU5Mg) ！

# 硬件
1. 树莓派3； 
2. 显示屏（拆自旧索尼笔记本，15.4寸，物理分辨率1366 x 768）；
3. 驱动板（淘宝）；
4. 单向透视镜（淘宝定制）；
5. 木框（淘宝定制）
6. 树莓派官方摄像头

建议：
1. 2&3可以依实际情况选择拆解显示器，或购买单屏成品，建议接口位于侧面并支持HDMI输入；
2. 可加装红外、压感等触摸板或购置触摸显示屏实现触摸功能。

# 软件
### 一、系统
1. 安装最新Raspbian with Pixel系统，务必注意安装图形化操作界面系统。
2. 基础设置
3. 打开终端，进行基本更新，包括替换源至国内。

### 二、聊天机器人
聊天机器人有多种选择，英文对话推荐使用Alexa 及 Gooogle Assistant（需要翻墙），中文对话可使用 up 主自制简易聊天机器人，拥有相应资质亦可尝试申请使用阿里云、百度等聊天机器人，有能力的可以自行开发。

#### Google Assistant
谷歌助手对树莓派支持良好，客制化程度高，没有语言及网络障碍情况下首推。安装后原生在后台运行。

通过与 IFTTT 进行联动，目前支持Yeelight智能灯具控制。

### 三、Home Assistant & Homebridge
智能家居系统的搭建详见本人于『少数派』发布的系列教程：https://sspai.com/post/38849

配合魔镜 iFrame 模块及触摸屏支持，可实现动态展示及操控。

**注：Home Assistant 本身是一个非常强大的平台，如果你具有开发能力，你会发现 HA 和 Magic Mirror很多时候可以实现相同的功能，取舍协调在于你自己。**

### 四、MagicMirror
Github: https://github.com/MichMich/MagicMirror

MM是一个模块化高度集成的魔镜项目，已经运营数年。客制化程度非常高。

### 五、文件清单：





