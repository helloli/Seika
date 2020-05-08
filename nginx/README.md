# nginx

## 下载与安装

下面将只示范 MacOS 下的 nginx 下载与安装：

1. 打开一个终端，输入 `brew -v` 确保已经安装 `Homebrew`，若没有安装，访问 [https://brew.sh/](https://brew.sh/) 按照说明安装
2. `brew install nginx` 安装 nginx，默认安装目录为 `/usr/local/etc/nginx`，可执行文件是 `/usr/local/bin/nginx`

## nginx 的基本操作

可以参考官方文档 [http://nginx.org/en/docs/beginners_guide.html](http://nginx.org/en/docs/beginners_guide.html)

1. `brew services start nginx` 或者 `/usr/local/bin/nginx` 启动 nginx 服务
4. 浏览器中访问 [http://localhost:8080](http://localhost:8080) 即可
5. 用 `brew services restart nginx` 或者 `nginx -s reload` 命令来重启 nginx

## nginx 的配置

如果是通过 `homebrew` 安装的 `nginx` 则可以通过 `brew info nginx` 查看安装信息。其中部分重要信息如下：

```
Docroot is: /usr/local/var/www

The default port has been set in /usr/local/etc/nginx/nginx.conf to 8080 so that
nginx can run without sudo.

nginx will load all files in /usr/local/etc/nginx/servers/.
```

### 配置文件

nginx 的配置文件在安装目录中，`/usr/local/etc/nginx/nginx.conf`，所有 `/usr/local/etc/nginx/servers/` 中的配置文件也都会被加载。而默认的文件目录为 `/usr/local/var/www`

#### 配置文件的结构

1. nginx 的配置文件由一个个指令组成，指令分为“简单指令”和“指令块”。其中“简单指令”由指令名+参数构成，用空格隔开，用分号结尾。比如 ``

## 配置 SSL 证书