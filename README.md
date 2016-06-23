####  项目依赖
      本项目依赖的库为ffmpeg。
####  主要功能
      1. 支持HLS播放。
      2. 支持MP4格式文件。
      3. 支持TS格式文件。
      4. 支持HLS,RTMP,rtsp直播。
####  ffmpeg编译步骤：
     1. 在终端执行  brew 命令。
     2. 安装yasm工具，执行 brew install yasm 命令。
     3. 执行 brew search yasm ，若安装成功则会显示一个成功标志。
     4. 下载gas-preprocessor 脚本，从 https://github.com/libav/gas-preprocessor
     5. 将gas-preprocessor.pl文件复制粘贴到 /usr/sbin/ 目录下(按commd+G快捷键，复制此路径) ,  若是根本就不能将这个文件复制到这个路径，我们需要换一个路径，/usr/local/bin/ 目录下，然后为文件开启可执行权限，打开终端输入以下命令行。
      chmod 777 /usr/local/bin/gas-preprocessor.pl
     6. 下载ffmpeg自动化编译脚本，从 https://github.com/kewlbear/FFmpeg-iOS-build-script
     7. 切换到下载目录，执行 ./build-ffmpeg.sh
     8. 最终将生成的FFmpeg-ios目录下的头文件和库文件替换到本工程ffmpeg下即可。

 
