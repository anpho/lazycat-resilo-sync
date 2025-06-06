# Resilo Sync for LazyCat Microserver.

[![LoadAndPack](https://github.com/anpho/lazycat-resilo-sync/actions/workflows/pack.yml/badge.svg)](https://github.com/anpho/lazycat-resilo-sync/actions/workflows/pack.yml)

[Resilo Sync][1] is a BitTorrent based file sharing tool. this is the raw project files used to build the lpk file for [LazyCat][2].

![](https://dl.lazycatmicroserver.com/appstore/metarepo/zh/apps/anpho.lzcapp.resilio/screenshots/ff1f60ae-1efa-4f8f-a45f-b35e5228a925.png!mod)

### Base Image

Resilo Sync's official [docker image][3], cached to LazyCat's registry for best performance.

### Download 

[LazyCat's AppStore][4] 

### How to build from 0

1. Retrive official docker image 
```
lzc-cli appstore copy-image resilio/sync
```
2. edit `lzc-manifest.yml`
3. Build and publish lpk. 
```
lzc-cli project build
lzc-cli appstore publish ./your-app.lpk
```

### Contact

[Twitter](https://x.com/anpho)


[1]:https://www.resilio.com/
[2]:https://lazycat.cloud/
[3]:https://hub.docker.com/r/resilio/sync
[4]:https://lazycat.cloud/appstore/#/shop/detail/anpho.lzcapp.resilio
