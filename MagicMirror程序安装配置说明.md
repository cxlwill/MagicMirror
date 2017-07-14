# 安装
背景：魔镜项目原则上可以运行在所有操作系统中，但必须具有图形化操作界面。如果是树莓派，系统推荐使用官方Raspbian with Pixel。
## 自动安装（仅限树莓派）
执行下列指令，则可自动安装：
`bash -c "$(curl -sL https://raw.githubusercontent.com/MichMich/MagicMirror/master/installers/raspberry.sh)"`

如果是国内网络环境，不建议使用上述安装指令，原因是到安装 Electron 部分注定卡死。

## 手动安装
1. 安装 Node.js 
2. 克隆魔镜项目`git clone https://github.com/MichMich/MagicMirror`
3. 转至安装文件夹`cd ~/MagicMirror`
4. 安装魔镜项目`npm install && npm start`

**注意：**如果使用SSH不要直接运行`npm start`，请使用`DISPLAY=:0 nohup npm start &`，或者安装VNC运行。

**国内被墙环境推荐使用cnpm**，安装：
`npm install -g cnpm --registry=https://registry.npm.taobao.org`
之后，将第4步替换为：
`cnpm install && cnpm start`
`cnpm` 支持 `npm` 除 `publish` 外其他所有指令

## 更新
转至魔镜项目所在文件夹：`cd ~/MagicMirror`
`git pull && npm install`
墙内：`git pull && cnpm install`

# 配置
1. 使用示例配置
复制文件，方法如下：
1.1 图形化页面直接操作：将 config/config.js.sample 重命名为 config.js
1.2 Linux 指令 

2. 环境配置
3. 模块配置


注：魔镜项目基于 Electron，在树莓派上，偶尔不稳定会闪退。



