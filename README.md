# w650_opencore_config 
#### 电脑配置
- cpu:i7-7700
- gpu:mx150+hd630(独显被屏蔽)

#### ToDo
- 加入蓝牙驱动,启动时间非常长,目前蓝牙未驱动
- 电池故障,电池未驱动  

#### 常用软件:
- clashx: https://github.com/yichengchen/clashX
- homebrew: https://brew.sh
- moom: https://xclient.info/s/moom.html  
- alfred: https://xclient.info/s/alfred.html  
- magnet: https://xclient.info/s/magnet.html
- appcleaner: https://freemacsoft.net/appcleaner/
- Qtopencoreconfig: https://github.com/ic005k/QtOpenCoreConfig
- hackintool: https://github.com/headkaze/Hackintool/releases

> brew install you-get youtube-dl mpv iina google-chrome telegram-desktop 
  
#### 问题与解答  
1. xcrun: error 
> xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun  
> 
> 解决方法  
> 重装xcode command line
> xcode-select --install
> 如果解决不了问题,执行一下命令
> sudo xcode-select -switch /
 
2. 任何源
> sudo spctl --master-disable

3. 
