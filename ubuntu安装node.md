# nodejs npm install

## apt 添加node仓库源
```sh
curl -sL https://deb.nodesource.com/setup_20.x | sudo -E bash -
```

跟新完毕后 `sudo apt update`

## 安装 nodejs npm

```sh
sudo apt install nodejs
```

## 检查
`node --version` | `npm --version`

## 升级npm
```sh
sudo npm install npm@latest -g
```
>! :warning:npm 安装请使用sudo

## 设置全局环境变量

先找到nodejs的位置 和npm modules的位置
```sh
which node
#我的安装位置出现在/usr/bin
npm root -g
#/usr/lib/node_modules
```
在/etc/profile || ~/.bashrc中配置
```sh
export NODE_HOME=/usr/bin
export NODE_PATH=/usr/lib/node_modules
export PATH=$NODE_HOME:$PATH
```

## 配置npm国内源

```sh
npm config set registry https://registry.npm.taobao.org
```

## 一键安装脚本
```sh
none
```

