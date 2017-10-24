# windows-nvm
windows下更新nodejs版本

## nvm下载

多版本nodejs管理工具nvm for windows [github资源下载链接](https://github.com/coreybutler/nvm-windows/releases)

选择对应位数的安装文件下载安装即可，安装过程中会出现几次弹窗询问是否对你本地已经安装的nodejs版本进行版本控制，点“是”就行了。

安装完成后，还需要对安装目录下的`setting.txt`文件进行修改，默认路径安装的情况下，setting.txt文件的存储路径为：`C:\Users\Administrator\AppData\Roaming\nvm`。（具体路径安装自己的安装路径而定）

打开setting.txt文件显示如下：

```
root: C:\Users\Administrator\AppData\Roaming\nvm
path: C:\Program Files\nodejs
```

修改为：

```
root: C:\Users\Administrator\AppData\Roaming\nvm
path: C:\Program Files\nodejs
arch: 64
proxy: none
node_mirror: https://npm.taobao.org/mirrors/node/
npm_mirror: https://npm.taobao.org/mirrors/npm/
```

保存后退出。

## nvm使用

通过nvm安装任意版本的node [nodejs官网查看版本](http://nodejs.cn/)

```
nvm install 8.7.0
```

安装完成后，运行`nvm use 8.7.0`去使用该版本

```
nvm use 8.7.0
```

然后输入

```
node -v
```

检查nodejs是否已更新到你想要的版本。

## 参考文章：

http://blog.csdn.net/qq_36423639/article/details/70230571