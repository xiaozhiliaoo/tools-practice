# 开发工具

brew:https://brew.sh/

git:brew install git

iterm2

mysql，mysql workbench

kafka，elk(es)，redis，MongoDB，Zookeeper

java14，maven，gradle

golang-go1.19

idea，pycharm，vscode

rust 【mdbook】

nodejs【blog】

sublime

DevToys

github必下载项目：blog,reading-note,interviews

# 辅助工具

DeepL

滴答清单

whiteboard白板

parallels desktop

RunCat

证券：东方财富，富途牛牛 ，老虎国际 ，富易 ，同花顺

亿图图示

有道云笔记

Adobe Acrobat Reader

calibre

Docker，Docker Desktop

draw.io

Mendeley Reference Manager

Tencent Lemon

WPS Office

Xmind

The Unarchiver

mermaidL: https://mermaid.live/edit#pako:eNqNVVtPE0EU_iubed4SsDe6iSYIPmoivJkmzbA7yMp2F3ZnDUhISpRaELXiHYhY7zFSiA-kFIg_xs62feIvODtntzdbNGnSnZlzvvOd75w5s4xUSyNIQQ5ZcImpkgkd37ZxNm1KEnapZbrZaWL7K8l1iB25cgVrWd1UJPb0Gavcr1U26tVf0rhNMCWTxCDYIb9zRZqxw-9nwlc4cWeKnbmMo84SzTWIrUjei6PmTr52cgJwgVdGtQyDqNTf3yh1AfgkuNvTYjO_pdT3PjcO8qz6PCSz32UbMIUYN8fkCUuVp8jtLDGp7D3aqu-_EFQ1S80s4PPTTfEZ_mccsBRrm9zhdIiW4Ro5VLfM3rxCUQo77KQKbBrlQ3b2slOMFny4DqKGy7-idJ0GfHhkvr2AIUh948jLrdYqVVYuee8rXAF-yNaOamdv_c2-stzlQSybc2kXcb--_YD_mrltLils9kmvFYObdmbazK3yI5EpdjWdRuaxDUwvrP3FcAKJJ21q0AUd8Oqsbmg8Qm8A3ZyxHKKGyCy_xsrHkfFZos4Ju-C8XS6I5BWKbGOvvwUg1U-ee-922c67xuH9MZ_CJHFcg45jw5jG6tz5aYEr1_j10Cu8auTWapXHsDw_Xe8q_wL-pyQggwjqfcx5e59BBtXPAXTg9YUT780BK35pBW5FbQs1qEkFfEhxE9KqVbY5-LR-z0_qqkhq09utsrffatVq4-tWY_1nc-1x_awM3p2n3u533jXN1-Xmhzft01cPvdLH1hIqC8vBnMBKCiQWosne-tdGKfCXJqxge2yGEnsMkuyaNn6ssK8GdX1nm19bJGqAKcxbZr2TjhWf-HV-XRZjY5UV8vV1rvUqDBJeatCRfdr2fpQiUoA5QSjWjRsW1WeW-uYNHS9Q2cFxxzySWveeYuo6PXNDgt2wwgNZQ-dCwpGAE7Dp1C0CaJdH_7M_BTRcmxZLV1WJ4_SZ2F18wClUZwqcpMGzOYAP0r0cBRmsaYvynG2Hz0ipl3PXC9EZFckoS-ws1jX-3C37PmlEZ0mWpJHCPzUyg_mlTqO0ucJN_cdvaslUkUJtl8jIndf4Exe8juEm4Q1o2dfhBRUPqYzmsYmUZbSIlJFYYiiaGk3FU6PRWDx5aURGS0iJxYdGotFoMhZNJmLDsWRyRUb3LItjDg-lYvF4Kp4YHUkkktFLyZRAuyUO_YArfwCdp73C

下载知识库：https://github.com/xiaozhiliaoo/reading-note ， https://github.com/xiaozhiliaoo/blog ，https://github.com/xiaozhiliaoo/interviews

Alfred

Postman

InsomniaX

zlibrary

PasteEasy

Kap mac下的录屏小软件

Typora

monoproxy 1q2w3e4r 账号77

# 常用脚本

## .bash_profile

```bash
JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-14.0.2.jdk/Contents/Home
CLASSPATH=$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
export M2_HOME=/Users/lili/Desktop/software/apache-maven-3.9.0
export JAVA_HOME
export CLASSPATH
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:$GOROOT/bin:$GOPATH:$GOBIN:$JAVA_HOME/bin:$M2_HOME/bin
export PATH=~/go/bin:$PATH
```

## .ssh目录下alert.sh

```bash
#!/bin/bash
cur_dir=$(pwd)

if [ $1 == 'github' ];then
    echo "choose github"
    git config --global user.name "xiaozhiliaoo"
    git config --global user.email "xiaozhiliaoo@gmail.com"
    cp -f $cur_dir/github/* $cur_dir
elif [ $1 == 'company' ];then
    echo "choose company"
    git config --global user.name "lili"
    git config --global user.email "lili@company.com"
    cp -f $cur_dir/company/* $cur_dir
else
     echo "no user"
fi

echo "user:`git config --global user.name`"
echo "email:`git config --global user.email`"
```

## 目录结构

```text
/Users/lili/Desktop/gitspace/github
/Users/lili/Desktop/gitspace/python-workspace
/Users/lili/Desktop/software
/Users/lili/Desktop/software/apache-maven-3.9.0
/Users/lili/Desktop/投资
/Users/lili/Desktop/国学
/Users/lili/Desktop/技术
/Users/lili/Desktop/其它
```

## git
```bash
git config --global user.name "lili"
git config --global user.email "772654204@qq.com"
ssh-keygen -t rsa -C "772654204@qq.com"
cat ~/.ssh/id_rsa.pub
配置到github上面去
ssh git@github.com
```
