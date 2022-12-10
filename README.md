# w650_opencore_config
Ventura
#### 电脑配置

- cpu:i7-7700
- gpu:mx150+hd630(独显被屏蔽)
- wifi:bcm4352

#### ToDo

* [ ] 电池故障,电池未驱动  

#### 常用软件与配置:

- 打开任何源：`sudo spctl --master-disable`

- Clashx: https://github.com/yichengchen/clashX

- [iDvel](https://github.com/iDvel)/**[rime-ice](https://github.com/iDvel/rime-ice)**

- Alfred: https://xclient.info/s/alfred.html#versions

- Moom: https://xclient.info/s/moom.html

- Homebrew: 

  - https://brew.sh
  - https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/

- Magnet: https://xclient.info/s/magnet.html

- Qtopencoreconfig: https://github.com/ic005k/QtOpenCoreConfig

- ohmyzsh: 
  `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

- hidpi: https://github.com/xzhih/one-key-hidpi

- App Cleaner: https://freemacsoft.net/appcleaner/

- The unarchiver: https://theunarchiver.com/

- Itlwm: https://github.com/OpenIntelWireless/itlwm

- Downie: https://xclient.info/s/downie.html

- Office : https://xclient.info/s/office-for-mac.html

- Typora: https://xclient.info/s/typora.html

- Dash: https://xclient.info/s/dash.html

- Tampermonkey: https://macapp.org.cn/app/tampermonkey.html

- App cleaner & uninstaller pro:https://xclient.info/s/app-cleaner-uninstaller-pro.html

- xcode: `xcode-select --install `

- 仓库内软件：

  ```bash
  brew install squirrel microsoft-edge telegram-desktop sublime-text visual-studio-code iterm2 karabiner-elements hackintool zsh-syntax-highlighting zsh-autosuggestions uninstallpkg   mpv iina eudic neovim intellij-idea miniconda snipaste 
  ```

- 可能需要的软件:
  ```bash
    brew install sogouinput you-get yt-dlp
  ```
#### 问题与解答  

1. xcrun: error 
> xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun  

> 解决方法  
> 重装xcode command line
> xcode-select --install
> 如果解决不了问题,执行一下命令
> sudo xcode-select -switch /

2. 交换option 和 command按键
> EFI/OC/kexts-voodooPS2Control.kext/contents/Plugins/voodooPs2keyboard.kext/contents/Info.plist/IOKitPersonalities/Platform Profile/Default/Swap command and option/YES

4. alfred最新版(tnt)不能用,改用旧版解决(新版已经解决）

5. 系统启动时间很长,根据代码发现是蓝牙驱动的问题,升级到特定的蓝牙驱动或者直接不加载蓝牙驱动(新驱动已经解决）

6. IntelliJ idea激活：[JETBRA.IN CHECKER | IPFS](https://3.jetbra.in/)

7. wifi驱动

   1. AirportBrcmFixup.kext/Contents/PlugIns/AirPortBrcmNIC_Injector.kext (true)
   2. AirportBrcmFixup.kext/Contents/PlugIns/AirPortBrcm4360_Injector.kext (false)

8. 蓝牙

   1. BlueToolFixup.kext (true)

   2. BrcmFirmwareData.kext (true)

   3. BrcmPatchRAM3.kext (true)

9. cpu变频

   1. CPUFriend.kext

      1. [CPUFriend/Instructions.md at master · acidanthera/CPUFriend (github.com)](https://github.com/acidanthera/CPUFriend/blob/master/Instructions.md)

         

10. 键盘驱动

    1. VoodooPS2Controller.kext (true)
    2. VoodooPS2Controller.kext/Contents/PlugIns/VoodooInput.kext (false)
    3. VoodooPS2Controller.kext/Contents/PlugIns/VoodooPS2Mouse.kext (true)
    4. VoodooPS2Controller.kext/Contents/PlugIns/VoodooPS2Keyboard.kext(true)
    5. VoodooPS2Controller.kext/Contents/PlugIns/VoodooPS2Trackpad.kext (true)
    6. VoodooRMI.kext (true)
    7. VoodooRMI.kext/Contents/PlugIns/RMII2C.kext (false)
    8. VoodooRMI.kext/Contents/PlugIns/RMISMBus.kext(false)
    9. VoodooRMI.kext/Contents/PlugIns/VoodooInput.kext (true)


#### 常用快捷键

- 显示隐藏文件：command+shift+.
- 显示路径栏：option+command+p
- 复制路径：option+command+c