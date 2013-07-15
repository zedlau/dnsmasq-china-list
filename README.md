# Dnsmasq-China-List （配置文件） #

## 简介 ##

越来越多的大陆境内网站使用智能 DNS 来给属于不同运营商的用户分配离他们最近的服务器，以达到访问提速的效果。但当我们使用国外 DNS 的时候（如8.8.8.8/4.2.2.1等），你所访问的网站将无法判断你是来自电信还是联通，因此你很可能被分配到非当前运营商的服务器上。当你使用电信宽带，而被分配到联通服务器上时，你很可能发现要打开你所访问的网站变得异常艰难。

Dnsmasq-China-List 是一个 Dnsmasq 的配置文件，使用这个配置文件，可以让 Dnsmasq 来修正因使用大陆境外 DNS 引起的部分境内网站的解析异常。

## 适用的平台 ##

* Mac OS X
* Ubuntu/Debian/Centos/Fedora/Archlinux 等

## 安装 Dnsmasq ##

### Mac OS X ###

1. 从 App Store 下载并 Xcode 
2. 安装 Homebrew (也可以用 MacPorts ，不过个人推荐 Homebrew)
3. 进入 Console （控制台）
4. 输入以下命令：

>brew install dnsmasq

### Ubuntu/Debian ###

未完待续

### CentOS/Fedora ###

未完待续

### ArchLinux ###

未完待续
