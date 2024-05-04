# use

## 设备

- MacBook Pro 14' M1 16GB

## Homebrew

- [官网](https://brew.sh/)

```bash
brew tap homebrew/cask-fonts
brew tap homebrew/cask-versions
brew tap buo/cask-upgrade
brew tap mongodb/brew
brew tap homebrew/autoupdate

# https://github.com/DomT4/homebrew-autoupdate，每 12 小时或启动系统时自动更新
brew autoupdate start 43200 --upgrade --cleanup --immediate --sudo

brew install git git-lfs git-flow
git config --global core.autocrlf false # 不自动转换 CRLF
git config --global core.quotepath off # 显示原始文件名
git config --global core.ignorecase false # 区分大小写
git config --global init.defaultBranch main
git config --global remote.origin.prune true # 自动移除不存在的远端分支
git config --global user.name username # 注意不要照抄
git config --global user.email email # 注意不要照抄

brew install btop
brew install fnm # manager Node.js version
brew install font-jetbrains-mono
brew install percona-toolkit # MySQL 运维工具
brew install php
brew install composer
brew install tldr # 像 man 命令一样在终端查看命令的说明和使用例子

# 访达插件
brew install --cask openinterminal # 在 Finder 打开终端，https://github.com/Ji4n1ng/OpenInTerminal，在访达随意右键到 Quick Actions 里添加工具栏按钮
brew install --cask qlmarkdown # 预览 Markdown
brew install --cask qlstephen # 预览没有扩展名的纯文本文件
brew install --cask --no-quarantine syntax-highlight # 代码高亮

brew install --cask another-redis-desktop-manager
brew install --cask font-hack-nerd-font
brew install --cask maczip
brew install --cask macs-fan-control # 控制风扇
brew install --cask picgo # 图床

brew tap mac-cleanup/mac-cleanup-py
brew install mac-cleanup-py # mac-cleanup [-c|-n]

# Go
brew install go

# 添加以下内容到 ~/.zshrc
export PATH="/Users/wangze/go/bin:$PATH"
export GO111MODULE=on
export GOPROXY=https://goproxy.cn


# Rust
curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
rustc -V && cargo -V

# vi ~/.cargo/config.toml
[source.crates-io]
replace-with = 'ustc'

[source.ustc]
registry = "git://mirrors.ustc.edu.cn/crates.io-index"


# Java
brew install maven
brew install jenv

# 添加以下内容到 ~/.zshrc
export PATH="$HOME/.jenv/bin:$PATH"
eval "$(jenv init -)"

jenv add xxx # 可以用 /usr/libexec/java_home 查看 xxx，一般在 /Library/Java/JavaVirtualMachines/zulu-18.jdk/Contents/Home
```

## App Store

- [Bitwarden](https://apps.apple.com/cn/app/bitwarden/id1352778147?l=en-GB&mt=12) 密码管理器
- [Bob](https://apps.apple.com/cn/app/bob-%E7%BF%BB%E8%AF%91%E5%92%8C-ocr-%E5%B7%A5%E5%85%B7/id1630034110?mt=12) 全局划词、截图 OCR 翻译
- [Command X](https://apps.apple.com/us/app/command-x/id6448461551?mt=12) 访达剪切文件快捷键
- [Gifski](https://apps.apple.com/cn/app/gifski/id1351639930?l=en-GB&mt=12) 视频转 Gif
- [PasteNow](https://apps.apple.com/us/app/pastenow-instant-clipboard/id1552536109) 跨设备剪切板
- [Quantumult X](https://apps.apple.com/lr/app/quantumult-x/id1443988620)
- [Telegram](https://apps.apple.com/cn/app/telegram/id747648890?l=en-GB&mt=12)
- [WPS Office](https://apps.apple.com/cn/app/wps-office/id1443749478?mt=12)
- [滴答清单](https://apps.apple.com/cn/app/%E6%BB%B4%E7%AD%94%E6%B8%85%E5%8D%95-%E4%B8%93%E6%B3%A8%E6%97%B6%E9%97%B4%E7%AE%A1%E7%90%86%E5%92%8C%E6%97%A5%E5%8E%86%E6%8F%90%E9%86%92%E4%BA%8B%E9%A1%B9/id966085870?mt=12)
- [腾讯会议](https://apps.apple.com/cn/app/tencent-meeting/id1484048379?l=en-GB)

## 软件

- [AlDente](https://github.com/AppHouseKitchen/AlDente-Charge-Limiter/releases) Charge Limiter
- [[Capslock]] 增强 Caps 键功能，先安装 [Karabiner-Elements](https://karabiner-elements.pqrs.org/docs/getting-started/installation/)
- [Chrome](https://www.google.com/intl/zh-CN/chrome/)
- [Clash Verge](https://github.com/clash-verge-rev/clash-verge-rev)
- [DBeaver Community](https://dbeaver.io/download/)
- [DevToys](https://github.com/DevToys-app/DevToysMac) 开发小工具集合，2022 年 9 月 18 日开始没维护
- [Dozer](https://github.com/Mortennn/Dozer) 隐藏菜单栏图标
- [IINA](https://iina.io/)
- [iTerm2](https://iterm2.com/)
- [JetBrains Toolbox](https://www.jetbrains.com/lp/toolbox/)
- [Kap](https://getkap.co/)  录屏和 Gif
- [Keyboardholder](https://keyboardholder.leavesc.com/) 自动切换输入法
- [Mac Mouse Fix](https://macmousefix.com/) 增强鼠标功能
- [MongoDB Compass](https://www.mongodb.com/try/download/compass)
- [Obsidian](https://obsidian.md/download) 双链笔记
- [Oh My Zsh](https://wangze.tech/Oh-My-Zsh)
- [OneDrive](https://www.microsoft.com/zh-cn/microsoft-365/onedrive/download)
- [OrbStack](https://orbstack.dev/dashboard) Docker 和虚拟机
- [Postman](https://www.postman.com/downloads/)
- [Raycast](https://www.raycast.com/) 启动器
- [Rectangle](https://rectangleapp.com/) 管理窗口布局
- [SwitchHosts](https://github.com/oldj/SwitchHosts/releases)
- [Snipaste](https://www.snipaste.com/download.html) 截图和贴图
- [Sourcetree](https://www.sourcetreeapp.com/) Git GUI
- [Tencent Lemon](https://lemon.qq.com/) 系统清理工具
- [Visual Studio Code](https://code.visualstudio.com/download)
- [whistle](https://wproxy.org/whistle/install.html) 抓包工具
- [Wireshark](https://www.wireshark.org/) 抓包工具（更多人推荐）
- [网易云音乐](https://music.163.com/#/download)
- [微信](https://mac.weixin.qq.com/?lang=zh_CN)
- [微信输入法](https://z.weixin.qq.com/)
- [微信开发者工具](https://developers.weixin.qq.com/miniprogram/dev/devtools/download.html)
- [支付宝小程序开发者工具](https://opendocs.alipay.com/mini/ide/download)

## 系统设置

- 打开
  - 三指拖移
  - 触控板手势 - 更多手势 -App Exposé - 四指向下清扫
  - 使窗口按应用程序成组
  - 使用大写锁定键切换“ABC”输入法
  - 在滚动条中点按跳到点按的位置
  - 键盘快捷键
    - 调度中心
      - 向左移动一个空间 Ctrl + Q
      - 向右移动一个空间 Ctrl + W
    - 调度中心：Ctrl + E
    - 应用程序窗口：Ctrl + D
  - Finder > Menu Bar > View > Show Path Bar
  - Privacy & Security > Extensions > Added extensions > OneDrive > Finder extensions

- 关闭
  - 自动切换到文稿的输入法
  - 调度中心 - 根据最近的使用情况自动重新排列空间
  - iCloud - 同步桌面与文稿文件夹
  - 在程序坞中显示最近使用的应用程序
  - Spotlight
  - Siri

## DNS

- [阿里云](https://www.alidns.com/knowledge?type=SETTING_DOCS#user_ios)
  - 主：`223.5.5.5`
  - 备：`223.6.6.6`
- [DNSPod](https://www.dnspod.cn/products/publicdns)
  - 主：`119.29.29.29`
  - 备：`182.254.116.116`

## Github

```bash
# ~/.ssh/config
Host github.com
    HostName ssh.github.com
    User {username}
    Port 443
```

## iCloud

```bash
# crontab -e 输入定时任务，确保 iCloud 同步正常
*/10 * * * * killall bird && killall cloudd
```

## Docker

```json
{
  "builder": {
    "gc": {
      "defaultKeepStorage": "10GB",
      "enabled": true
    }
  },
  "experimental": false,
  "log-driver": "json-file",
  "log-opts": {
    "max-file": "1",
    "max-size": "10m"
  }
}
```

## Chrome

- 访问一次 [google.com/ncr](https://google.com/ncr)，避免 Google 自动重定向
- 设置扩展允许预加载网页：`uBlock Origin`，`Decentraleyes`
- F12 进入 DevTools，Setting > Experiments > Redesign of the filter bar in the Network Panel，关闭，效果：
  - ![image.png](https://cdn.jsdelivr.net/gh/11ze/static/images/20240428233857.png)
