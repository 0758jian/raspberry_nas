### 树莓派4B 装好openMediaVault nas系统后，docker-compose 布署应用
- qbittorrent： BT PT下载
- transmission： BT PT下载
- aria2： 普通下载
- nextcloud：个人私有云
- bitwarden：密码管理（强推）
- frp：内网穿透
- nginx：主要用于https访问，反代到各应用上
### clone下来后，frp、nginx的配置信息，根据实际自行修改
### 使用方式，根据实际配置.env里的参数
```
    git clone https://github.com/0758jian/raspberry_nas.git raspberry
    cd raspberry
    cp .env.example .env
    sudo docker-compose up -d
```

- TG技术群：https://t.me/joinchat/LqcgBEUJ7133BFBEv67NCw