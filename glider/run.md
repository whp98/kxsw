# glider 常用使用

协议转换工具

## ws+tls 转 ss

```
./glider -verbose -listen ss://chacha20-ietf-poly1305:qazwsxedc@:30202 -forward  "tls://v2-19.ssrsub.xyz:443?skipVerify=true,ws://,vmess://1a662efb-4780-4721-bc5a-225374d7cf00@?alterID=233"

```

## socks5 转 ss

```
nohup ./glider -verbose -listen ss://chacha20-ietf-poly1305:qazwsxedc@:30200 > /dev/null &

```

## vmess 转 socks5

```
./glider -verbose  -listen :30202  -forward tls://t84d3dxr9.hk-hgc.tradewind.link:443,ws://@/je5x3pBN1vez3NQudNkB,vmess://12d637b1-b8aa-469c-ad4a-fd556160413d@?alterID=0

```

