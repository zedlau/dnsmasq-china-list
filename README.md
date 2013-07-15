# Dnsmasq-China-List （配置文件） #

## 简介 ##

越来越多的大陆境内网站使用智能 DNS 来给属于不同运营商的用户分配离他们最近的服务器，以达到访问提速的效果。但当我们使用国外 DNS 的时候（如8.8.8.8/4.2.2.1等），你所访问的网站将无法判断你是来自电信还是联通，因此你很可能被分配到非当前运营商的服务器上。当你使用电信宽带，而被分配到联通服务器上时，你很可能发现要打开你所访问的网站变得异常艰难。

Dnsmasq-China-List 是一个 Dnsmasq 的配置文件，使用这个配置文件，可以让 Dnsmasq 来修正因使用大陆境外 DNS 引起的部分境内网站的解析异常。

## 适用的平台 ##

* Mac OS X
* Ubuntu/Debian/Centos/Fedora/Archlinux 等

## 安装 Dnsmasq ##

### Mac OS X ###

1. 从 App Store 下载并安装 Xcode 
2. 安装 Homebrew (也可以用 MacPorts ，不过个人推荐 Homebrew 。注意，这两个只能选其一，否则会冲突。)
3. 进入 Console （控制台）
4. 输入以下命令（根据提示操作完成安装）：

> brew install dnsmasq

### Ubuntu/Debian ###

> sudo apt-get install dnsmasq

### CentOS/Fedora ###

> sudo yum -y install dnsmasq

### ArchLinux ###

> sudo pacman -S dnsmasq

## 配置 Dnsmasq ##

未完待续

## 自我诊断与维护 ##

如果发现访问某个大陆境内网站十分缓慢，可以通过以下两个命令进行自我诊断：

>dig @8.8.8.8 domain.com +short
>
>dig @114.114.114.114 domain.com +short

如果得到的 IP 不一致，则可以将该域名添加到 server.conf 中并重启 Dnsmasq 。

如：

>MacPro:~ Zed$ dig @8.8.8.8 51buy.com +short
>
>112.64.234.138
>
>MacPro:~ Zed$ dig @114.114.114.114 51buy.com +short
>
>101.226.49.43

如果方便的话也可以同时反馈到 zedlau#me.com 。
