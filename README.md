# woccloud_qv2ray
适用于卧槽云加速的qv2ray科学上网梯子，适用于Ubuntu20.04，可以解决需要手动打开代理的问题

### 使用方法

1. 在创建文件夹：mkdir  /home/**xxx**/.config/qv2ray，其中**xxx**为自己的电脑用户名

2. 下载克隆本项目到刚刚创建的文件夹下

3. 修改Qv2ray.conf文件中的内容，将**xxx**改为自己的电脑用户名：

   "v2AssetsPath_linux": "/home/**xxx**/.config/qv2ray/vcore/",

   "v2CorePath_linux": "/home/**xxx**/.config/qv2ray/vcore/v2ray"

4. 修改groups.json文件中的内容     

   "address": "**xxxxxxxxxxxx**"，将**xxxxxxxxxxxx**修改为自己的订阅链接

5. 创建快捷方式，修改qv2ray.desktop文件内容，将**xxx**改为自己的电脑用户名，保存并退出

   Exec=/home/**xxx**/.config/qv2ray/Qv2ray.AppImage
   Icon=/home/**xxx**/.config/qv2ray/qv2ray.512.png

6. 在/home/**xxx**/.config/qv2ray目录下打开终端，输入命令：

   sudo chmod +x qv2ray.desktop

   sudo cp qv2ray.desktop /usr/share/applications
