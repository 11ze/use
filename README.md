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

# https://github.com/DomT4/homebrew-autoupdate，每12小时或启动系统时自动更新
brew autoupdate start 43200 --upgrade --cleanup --immediate --sudo

brew install git git-lfs git-flow
git config --global core.autocrlf false # 不自动转换CRLF
git config --global core.quotepath off # 显示原始文件名
git config --global core.ignorecase false # 区分大小写
git config --global init.defaultBranch main
git config --global remote.origin.prune true # 自动移除不存在的远端分支
git config --global user.name username # 注意不要照抄
git config --global user.email email # 注意不要照抄
git config --global credential.github.com.provider username # 注意不要照抄

# 访达插件
brew install openinterminal # 在Finder打开终端，https://github.com/Ji4n1ng/OpenInTerminal，在访达任意地方右键，到Quick Actions里添加工具栏按钮
brew install qlmarkdown # 预览Markdown
brew install qlstephen # 预览没有扩展名的纯文本文件
brew install syntax-highlight # 代码高亮

brew install another-redis-desktop-manager
brew install bruno # API客户端
brew install btop
brew install dbeaver-community # 暂不用
brew install fnm # 管理Node.js版本
brew install font-hack-nerd-font
brew install font-jetbrains-mono
brew install iina # 媒体播放器
brew install iterm2
brew install kap # 录屏和Gif
brew install mac-mouse-fix # 增强鼠标功能
brew install maczip
brew install mini-program-studio # 支付宝小程序开发者工具
brew install neteasemusic # 网易云音乐
brew install picgo # 图床
brew install obsidian # 双链笔记
brew install postman # API客户端
brew install raycast # 启动器
brew install rectangle # 管理窗口布局
brew install snipaste # 截图和贴图
brew install sourcetree # Git GUI
brew install switchhosts
brew install tldr # 像man命令一样在终端查看命令的说明和使用例子，可设置别名alias iman='tldr'
brew install wechatwebdevtools # 微信开发者工具

brew tap mac-cleanup/mac-cleanup-py
brew install mac-cleanup-py # mac-cleanup [-c|-n]

# PHP
brew install composer
brew install php

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

# 添加以下内容到~/.zshrc
export PATH="$HOME/.jenv/bin:$PATH"
eval "$(jenv init -)"

jenv add xxx # 可以用/usr/libexec/java_home查看xxx，一般在/Library/Java/JavaVirtualMachines/zulu-18.jdk/Contents/Home
```

## App Store

- [Bob](https://apps.apple.com/cn/app/bob-%E7%BF%BB%E8%AF%91%E5%92%8C-ocr-%E5%B7%A5%E5%85%B7/id1630034110?mt=12) - 全局划词、截图OCR翻译
- [Command X](https://apps.apple.com/us/app/command-x/id6448461551?mt=12) - 访达剪切文件快捷键
- [Gifski](https://apps.apple.com/cn/app/gifski/id1351639930?l=en-GB&mt=12) - 视频转Gif
- [iBar](https://apps.apple.com/cn/app/ibar-menubar-icon-control-tool/id6443843900?l=en-GB&mt=12) - 隐藏菜单栏图标
- [PasteNow](https://apps.apple.com/us/app/pastenow-instant-clipboard/id1552536109) - 跨设备剪切板
- [Quantumult X](https://apps.apple.com/lr/app/quantumult-x/id1443988620)
- [Telegram](https://apps.apple.com/cn/app/telegram/id747648890?l=en-GB&mt=12)
- [WPS Office](https://apps.apple.com/cn/app/wps-office/id1443749478?mt=12)
- [滴答清单](https://apps.apple.com/cn/app/%E6%BB%B4%E7%AD%94%E6%B8%85%E5%8D%95-%E4%B8%93%E6%B3%A8%E6%97%B6%E9%97%B4%E7%AE%A1%E7%90%86%E5%92%8C%E6%97%A5%E5%8E%86%E6%8F%90%E9%86%92%E4%BA%8B%E9%A1%B9/id966085870?mt=12)
- [腾讯会议](https://apps.apple.com/cn/app/tencent-meeting/id1484048379?l=en-GB)

## 软件

- [AlDente](https://github.com/AppHouseKitchen/AlDente-Charge-Limiter/releases) - 控制笔记本电池充电和放电
- [Capslock](https://wangze.tech/Capslock%EF%BC%9A%E5%A2%9E%E5%BC%BAMac%E7%9A%84Caps%E9%94%AE%E5%8A%9F%E8%83%BD) - 增强Caps键功能
- [Chrome](https://www.google.com/intl/zh-CN/chrome/)
- [JetBrains Toolbox](https://www.jetbrains.com/lp/toolbox/)
- [Navicat Premium Lite](https://www.navicat.com/en/download/navicat-premium-lite#macos) - 数据库管理工具，免费
- [Oh My Zsh](https://wangze.tech/Mac%E5%AE%89%E8%A3%85oh-my-zsh)
- [OneDrive](https://www.microsoft.com/zh-cn/microsoft-365/onedrive/download)
- [OrbStack](https://orbstack.dev/dashboard) - Docker和Linux 虚拟机
- [Tencent Lemon](https://lemon.qq.com/) - 系统清理工具
- [Visual Studio Code](https://code.visualstudio.com/download)
- [微信](https://mac.weixin.qq.com/?lang=zh_CN)
- [微信输入法](https://z.weixin.qq.com/)

## 工具网站

- [IT Tools - Handy online tools for developers](https://it-tools.tech/)
- [帮小忙，腾讯 QQ 浏览器在线工具箱平台](https://tool.browser.qq.com/)

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
  - 调度中心 - 根据最近的使用情况自动重新排列空间
  - iCloud - 同步桌面与文稿文件夹
  - 在程序坞中显示最近使用的应用程序
  - Spotlight
  - Keyboard > Service > Text > Search man Page Index in Terminal

## DNS

- [DNSPod](https://www.dnspod.cn/products/publicdns)：`119.29.29.29`
- [阿里云](https://www.alidns.com/knowledge?type=SETTING_DOCS#user_ios)：`223.5.5.5`

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
# crontab -e定时kill iCloud进程，会自动重启，确保iCloud同步正常
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

- 访问一次 [google.com/ncr](https://google.com/ncr)，避免Google自动重定向
- 设置扩展允许预加载网页：uBlock Origin，Decentraleyes
- F12 进入 DevTools，Setting > Experiments > Redesign of the filter bar in the Network Panel，关闭，效果：
  - ![image.png](https://cdn.jsdelivr.net/gh/11ze/static/images/20240428233857.png)
