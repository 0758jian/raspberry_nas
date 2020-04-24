### 树莓派4B 装好openMediaVault nas系统后，docker-compose 布署应用
- qbittorrent： BT PT下载
- transmission： BT PT下载
- aria2： 普通下载
- nextcloud：个人私有云
- bitwarden：密码管理（强推）
- frp：内网穿透
- jellyfin 这个大文件视频，性能就呵呵了。已经配openOMX了
- nginx：主要用于https访问，反代到各应用上
### clone下来后，frp、nginx的配置信息，根据实际自行修改
- mysql 目前只有nextcloud结合使用，当然你也可以加个wordpress容器用
- acme 目录是放置相关域名的证书地方
### 使用方式，根据实际配置.env里的参数
- 建议先在portainer上先pull所需要的镜像再启用
- 注意先配置好移动硬盘上的目录
```
    git clone https://github.com/0758jian/raspberry_nas.git raspberry
    cd raspberry
    cp .env.example .env
    sudo docker-compose up -d
```

- TG技术群：https://t.me/joinchat/LqcgBEUJ7133BFBEv67NCw