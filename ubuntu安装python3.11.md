# ubuntu 安装python3.11

[🌐如何在Ubuntu22.04中安装python3.11How To Install Python 3.11 on Ubuntu, Debian and LinuxMint](https://www.linuxmi.com/python-3-11.htmlhttps://tecadmin.net/how-to-install-python-3-11-on-ubuntu/)

>! :warning:里面提供两种方法安装python

对于Ubuntu 22.04，Ubuntu20.04，Ubuntu 18.04 及其衍生版本，如 Linux Mint，有一个流行的 Deadsnakes PPA 维护Python 3.11以及其他Python版本的软件包。

注意：PPA 不支持 Ubuntu 22.10。您可以按照底部链接从源码压缩包构建它。
```sh
sudo add-apt-repository ppa:deadsnakes/ppa
```

更新包管理器
```bash
sudo apt update
```

安装python3.11
```sh
sudo apt install python3.11 -y
```
`python3.11 -version` 检查是否安装成功

安装pip
```sh
curl -sS https://bootstrap.pypa.io/get-pip.py | python3.11 
```

使用pip下载包 检验是否可用
```sh
python3.11 -m pip install rich
#进入python3.11
python3.11 
#导入包
import rich
#如没有错误弹出表示成功
```



