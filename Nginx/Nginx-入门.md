# Nginx笔记-入门

## 一、Nginx 简介

### 1. Nginx 是什么？

Nginx 是一个高性能的HTTP和反向代理web服务器，同时也提供了IMAP/POP3/SMTP服务。



## 二、Nginx 安装

环境说明：

1. CentOS 7
2. Nginx 1.16.1

安装步骤：

1. 下载Nginx稳定版本 : wget http://nginx.org/download/nginx-1.16.1.tar.gz
2. 解压 ： tar -xvf nginx-1.16.1.tar.gz
3. 配置：./configure --prefix=/export/server/nginx
4. 编译：

```shell
$ wget http://nginx.org/download/nginx-1.16.1.tar.gz
$ tar -xvf nginx-1.16.1.tar.gz
$ mkdir nginx
$ cd nginx-1.16.1
$ ./configure --prefix=/export/server/nginx
$ sudo yum -y install gcc gcc-c++ pcre-devel openssl openssl-devel zlib-devel
$ ./configure --prefix=/export/server/nginx
$ make
$ make install

[admin@JD nginx]$ pwd
/export/server/nginx
[admin@JD nginx]$ ll
total 0
drwxrwxr-x 2 admin admin 333 Dec 22 00:34 conf
drwxr-xr-x 2 admin admin  40 Dec 22 00:34 html
drwxrwxr-x 2 admin admin   6 Dec 22 00:27 logs
drwxrwxr-x 2 admin admin  19 Dec 22 00:34 sbin
[admin@JD nginx]$
```



### 3. 解决问题

#### 3.1 编译失败：./configure: error: C compiler cc is not found

```
[admin@JD nginx]$ ./configure 
checking for OS
 + Linux 3.10.0-957.el7.x86_64 x86_64
checking for C compiler ... not found

./configure: error: C compiler cc is not found
```



### 4. 参考资料

1. http://nginx.org/en/docs/install.html
2. http://nginx.org/en/docs/configure.html

## 三、Nginx 实战演示

## 四、Nginx 配置文件

## 五、Nginx 原理