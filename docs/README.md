# docsify-template

## 说明
整理的docsify 模板，主要包括：

* [X] 主题
* [X] 分页
* [X] 搜索
* [X] 最后编辑时间
* [X] github 挂件
* [X] edit in repo

## 获取步骤

### 安装node

```batch
# 首先安装必要的环境
yum install gcc gcc-c++

# 下载
wget https://npm.taobao.org/mirrors/node/v13.0.1/node-v13.0.1-linux-x64.tar.gz
# 解压并重命名文件夹
tar -xvf  node-v13.0.1-linux-x64.tar.xz
mv node-v13.0.1-linux-x64 node

# 配置环境变量
vim /etc/profile
# -----------------------------------------
#set for nodejs  
export NODE_HOME=/usr/local/node  
export PATH=$NODE_HOME/bin:$PATH
# -----------------------------------------

# 使配置文件生效
source /etc/profile

# 成功后查看版本
node -v
npm -v 
```

### 安装docsify

```batch
```

### 安装git

```batch
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

### 克隆项目并生成

