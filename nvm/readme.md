# nvm

> node 的版本管理工具，可以通过 nvm 来切换不同的 node 版本。

## install

- macos 或者 Linux 安装或更新 nvm 可以使用 curl 或者 wget 命令

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

```shell
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

- windows 系统可以使用 [nvm-windows](https://github.com/coreybutler/nvm-windows/releases) 来下载最新的安装包安装使用 nvm

## used

1. 下载对应的 node 版本；node 是最新版本的别名，也可以指定 node 的具体版本下载如：14.0.0

   ```shell
   nvm install node
   ```

2. 查看可安装的 node 版本

   ```shell
   nvm list available
   ```

3. 查看当前已安装的 node 版本

   ```shell
   nvm ls
   ```

4. 使用 node 版本

   ```shell
   nvm use <version>
   ```

5. 卸载已安装的 node 版本

   ```shell
   nvm uninstall <version>
   ```

6. 国内下载 node 版本会很慢可以设置对应国内的镜像源

   - 使用命令行

     ```shell
     nvm node_mirror https://npmmirror.com/mirrors/node/
     nvm npm_mirror https://npmmirror.com/mirrors/npm/
     ```

   - 修改 nvm安装路径下/setting 文件

     ```txt
     node_mirror https://npmmirror.com/mirrors/node/
     npm_mirror https://npmmirror.com/mirrors/npm/
     ```
