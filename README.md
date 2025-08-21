官方发布站：https://taoiptv.com

程序运行环境：python3 + mysql, 步骤如下：

第1步：新建数据iptv,执行初始脚本data/iptv_data.sql
修改python3 hotels.py、python3 multicast.py、python3 iptvdata.py中数据库配置

第2步：对于Ubuntu/Debian的Linux发行版系统，以下2行命令安装FFmpeg：
sudo apt update、sudo apt install ffmpeg（其他系统安装FFmpeg，自行搜索教程）

第3步：安装好python环境，安装python依赖模块，使用以下3行命令安装：
pip3 install bs4、pip3 install m3u8、pip3 install requests（其他运行中缺少模块，可自行安装）

第4步：修改组播抓取配置，执行主程序
修改multicast.py中113行api_token，执行python3 main.py，执行完成，生成source/iptv.txt直播源文件
