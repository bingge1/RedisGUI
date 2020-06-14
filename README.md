### 编译依赖
* 安装Nodejs 语言安装包
* 安装Python 环境，要求2.7版本，不可使用3.x版本
* [net framework 2.0 sdk](https://www.microsoft.com/en-us/download/details.aspx?id=15354) 或者visual studio

npm config set registry http://registry.npm.taobao.org/


npm config set msvs_version 2017 --global

npm install --global --production  windows-build-tools --vs2017


3、克隆sea代码仓库
git clone  git.atkj6666.com/blockchain/sea
4、到仓库根目录下执行安装依赖
npm install
electron-rebuild .
 electron-builder install-app-deps
5、启动sea客户端
npm start



打包命令
electron-packager . sea --win --out dist --arch=x64 --version1.0.0 --overwrite --icon=./static/img/icon.png

打包之后，使用cmd 下面的start$env 脚本启动

npm install -g electron-packager
npm run package

安装指南

将压缩包 解压到 D盘合适目录 下