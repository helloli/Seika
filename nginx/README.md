# nginx

## 下载与安装

下面将只示范 MacOS 下的 nginx 下载与安装：

1. 打开一个终端，输入 `brew -v` 确保已经安装 `Homebrew`，若没有安装，访问 [https://brew.sh/](https://brew.sh/) 按照说明安装
2. `brew install nginx` 安装 nginx，安装默认目录为 `/usr/local/etc/nginx`，可执行文件是 `/usr/local/bin/nginx`

## nginx 的基本操作

可以参考官方文档 [http://nginx.org/en/docs/beginners_guide.html](http://nginx.org/en/docs/beginners_guide.html)

1. `brew services start nginx` 或者 `/usr/local/bin/nginx` 启动 nginx 服务
4. 浏览器中访问 [http://localhost:8080](http://localhost:8080) 即可
5. 用 `brew services restart nginx` 或者 `nginx -s reload` 命令来重启 nginx

## nginx 的配置

## 配置 SSL 证书