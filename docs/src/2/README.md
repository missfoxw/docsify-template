
本文测试环境：`centos7.5`

## 使用模板

克隆项目。
> `git clone`支持多种协议，如`http(s)`,`ssh`,`git`等。

```bash
git clone git://github.com/missfoxw/docsify-template.git
```

## 启动前的依赖

### 安装node

> docsify需要node环境，node自带npm

```bash
# 以下使用二进制文件安装，该部署过程使用的安装包是已编译好的二进制文件。解压之后，在bin文件夹中就已存在node和npm，无需重复编译。

# 下载（可指定版本）
wget https://npm.taobao.org/mirrors/node/v13.0.1/node-v13.0.1-linux-x64.tar.xz

# 解压并重命名文件夹
tar -xvf  node-v13.0.1-linux-x64.tar.xz
mv node-v13.0.1-linux-x64 node

# 确认安装目录
cd node
pwd
/opt/setup/node

# 创建软链接，就可以在任意目录下直接使用node和npm命令
ln -s /opt/setup/node/bin/node /usr/local/bin/node
ln -s /opt/setup/node/bin/npm /usr/local/bin/npm

# 查看node、npm版本
node -v
npm -v 
```

### 安装docsify

```bash
npm i docsify-cli -g
```

### 安装git

使用git方便管理文档

```bash
# 首先安装必要的环境
yum install curl-devel expat-devel gettext-devel openssl-devel zlib-devel gcc perl-ExtUtils-MakeMaker

# 删除已有git
yum remove git

# 然后下载安装包解压等
cd /opt/free/git
wget https://www.kernel.org/pub/software/scm/git/git-2.9.3.tar.gz
tar -zxvf git-2.9.3.tar.gz
mv git-2.9.3.tar git

# 配置git安装路径
cd /opt/free/git/git
./configure prefix=/usr/local/git/

# 编译安装
make && make install

# 配置环境变量
vim /etc/profile
# -----------------------------------------
#set for git
export PATH=/usr/local/git/bin:$PATH
# -----------------------------------------

# 使配置文件生效
source /etc/profile

# 成功后查看版本
git --version
```

## 启动模板

在`docsify-template`目录下启动模板：

```bash
# 打开下载的地址

docsify serve docs
```
访问地址:`http://localhost:3000`

[点我看看](http://118.190.97.56:3000)
