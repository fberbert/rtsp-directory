## RTSP Directory

This repository contains a list of RTSP URLs for various IP camera models. The URLs are presented in a table format. The table below contains the following:

- **IP camera models** (column 1)
- **RTSP URLs** (column 2)

## How to discover my local camera IP address?

### Method 1: Router

1. Access your router's admin panel.
2. Look for a section called "connected devices" or similar.
3. Look for your camera's IP address.

### Method 2: IP Scanner

1. On Linux you can use `nmap`:

```bash
nmap -p 554 --open x.x.x.x/24
```

Where `x.x.x.x` is your local network IP address, and `/24` is the subnet mask. The `-p 554` flag is used to scan for devices on port 554, which is the default port for RTSP. And the `--open` flag is used to show only open ports.

You will get a list of devices with the port 554 open, which are likely to be cameras, like this:

```
Nmap scan report for 192.168.68.100
Host is up (0.020s latency).

PORT    STATE SERVICE
554/tcp open  rtsp

Nmap scan report for 192.168.68.102
Host is up (0.11s latency).

PORT    STATE SERVICE
554/tcp open  rtsp

Nmap scan report for 192.168.68.103
Host is up (0.065s latency).

PORT    STATE SERVICE
554/tcp open  rtsp

Nmap scan report for 192.168.68.109
Host is up (0.045s latency).

PORT    STATE SERVICE
554/tcp open  rtsp

Nmap done: 256 IP addresses (14 hosts up) scanned in 11.02 seconds
```

### Method 3: You camera's software

1. Open your camera's software.
2. Look for a section called "network" or similar.
3. Look for your camera's IP address.

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
