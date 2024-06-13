## RTSP Directory

This repository contains a list of RTSP URLs for various IP camera models. The URLs are presented in a table format. The table below contains the following:

- **IP camera models** (column 1)
- **RTSP URLs** (column 2)

## Generic models

Try this first:

### Generic RTSP 1

```
rtsp://[IP-ADDRESS]:554/user=admin&password=[PASSWORD]&channel=1&stream=0.sdp
```

Confirmed working on:
- ICsee app

### Generic RTSP 2

```
rtsp://admin:[PASSWORD]@[IP-ADDRESS]:554/onvif1
```

Confirmed working on:
- Yoosee app

### Generic RTSP 3

```
rtsp://admin:[PASSWORD]@[IP-ADDRESS]:554/h264?channel=1
```

Confirmed working on:
- ???

### Generic RTSP 4

```
rtsp://admin:[PASSWORD]@[IP-ADDRESS]:554
```

Confirmed working on:
- ???

### Intelbras

```
rtsp://admin:[PASSWORD]@[IP-ADDRESS]:554/cam/realmonitor?channel=1&subtype=0&unicast=true&proto=Onvif
```
```
rtsp://[DOMAIN]:[PORT]/user=[USERNAME]&password=[PASSWORD]&channel=1&stream=0.sdp
```


### Tecvoz

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/profile1
```

### DVR/NVR - TW Line - Tecvoz

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/chID=1&streamType=main&linkType=tcpa
```

### DVR/NVR - T1/THK Line - Tecvoz

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/Streaming/Channels/01
```

### DVR/NVR - TVZ

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/user=USERNAME&password=PASSWORD&channel=1&stream=0.sdp
```

### IP Cameras - Tecvoz TV (Future)

```
rtsp://[IP-ADDRESS]:PORT/user=USERNAME&password=PASSWORD&channel=1&stream=1
```

### Cameras - Line T1/THK - Tecvoz

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/Streaming/Channels/101
```

### Cameras - Line ICB Intelligent - Tecvoz

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/mode=real&idc=1&ids=1
```

### Alive

```
rtsp://[IP-ADDRESS]:PORT/user=USERNAME&password=PASSWORD&channel=1&stream=0.sdp?real_stream
```

### Axis

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/axis-media/media.amp?videocodec=h264
```

### Clear

```
rtsp://[IP-ADDRESS]:PORT/user=USERNAME&password=PASSWORD&channel=1&stream=0.sdp
```

### Dahua

```
rtsp://[DOMAIN]:[PORT]/user=[USERNAME]&password=[PASSWORD]&channel=1&stream=0.sdp
```

### Foscam

```
rtsp://[USERNAME]:[PASSWORD]@[IP-ADDRESS]:PORT/videoMain
```

### Greatek

```
rtsp://[DOMAIN]:[PORT]/user=[USERNAME]&password=[PASSWORD]&channel=1&stream=0.sdp
```

GIGA:
```
rtsp://DOMINIO:PORTA/user=USUARIO&amp;password=SENHA&amp;channel=1&amp;stream=0.sdp
```

```
rtsp://DOMINIO:PORTA/user=USUARIO&password=SENHA&channel=1&stream=0.sdp
```

HDL:
```
rtsp://DOMINIO:PORTA/user=USUARIO&password=SENHA&channel=1&stream=0.sdp
```

HIKVISION:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/h264/ch1/main/av_stream
```

HEROSPEED DVR:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/snap.jpg
```

JFL:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/h264/ch1/main/av_stream
```


JORTAN:
```
rtsp://DOMINIO:PORTA/user=USUARIO&password=SENHA&channel=1&stream=0.sdp
```

LG:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/Master-0
```

LUXVISION:
```
rtsp://DOMINIO:PORTA/user=USUARIO&password=SENHA&channel=1&stream=0.sdp
```

MULTILASER:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/H264?ch=1&subtype=0
```

VENETIAN:
```
rtsp://DOMINIO:PORTA/user=USUARIO&password=SENHA&channel=1&stream=0.sdp?
```

```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/cam/realmonitor?channel=1&subtype=0&unicast=true&proto=Onvif
```

VIVOTEK:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/live.sdp
```

TWG:
```
rtsp://DOMINIO:PORTA/user=USUARIO&password=SENHA&channel=1&stream=0.sdp?
```

ZAVIO:
```
rtsp://USUARIO:SENHA@DOMINIO:PORTA/video.pro1
```
