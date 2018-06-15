# nginx-vod-module appdemo

> i reference `[nginx-vod-module-docker](https://github.com/NYTimes/nginx-vod-module-docker)` && build  with docker && docker-compose

## How to build image

```code
docker build -t dalongrong/myvod-nginx
```

## Run demo

* Run

```code
cd demo && docker-compose up -d

open http://hostip  for test
```

* hls&&dash&&thumb

```code
- hls: http://hostip/hls/<videosname>/master.m3u8
- dash: http://hostip/hls/<videosname>/manifest.mpd
- Thumbnail: http://hostip/thumb/<videosname>/thumb-<index>.jpg
```

## docs

- [nginx-vod-module](https://github.com/kaltura/nginx-vod-module)
- [nginx-vod-module-docker](https://github.com/NYTimes/nginx-vod-module-docker)
