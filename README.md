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
- magnet: https://xclient.info/s/magnet.html
- Qtopencoreconfig: https://github.com/ic005k/QtOpenCoreConfig
- ohmyzsh: sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

> xcode-select --install 

> brew install you-get youtube-dl mpv iina google-chrome telegram-desktop sublime-text visual-studio-code iterm2 karabiner-elements hackintool zsh zsh-syntax-highlighting zsh-autosuggestions uninstallpkg 

#### 问题与解答  

1. xcrun: error 
> xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun  
 
> 解决方法  
> 重装xcode command line
> xcode-select --install
> 如果解决不了问题,执行一下命令
> sudo xcode-select -switch /

2. 任何源
> sudo spctl --master-disable

3. 交换option 和 command按键
> EFI/OC/kexts-voodooPS2Control.kext/contents/Plugins/voodooPs2keyboard.kext/contents/Info.plist/IOKitPersonalities/Platform Profile/Default/Swap command and option/YES

4. alfred最新版(tnt)不能用,改用旧版解决
5. 系统启动时间很长,根据代码发现是蓝牙驱动的问题,升级到特定的蓝牙驱动或者直接不加载蓝牙驱动
