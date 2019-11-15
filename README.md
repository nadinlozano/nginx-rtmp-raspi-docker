# nginx-rtmp-raspi-docker
Docker image with Nginx using the nginx-rtmp-module for Raspberry Pi

## Usage
Build an image:
``` docker build -t nginx-rtmp-raspi -f Dockerfile .```

Run a container:
```docker run -d --name nginx-rtmp-raspi -p 1935:1935 nginx-rtmp-raspi```

URL to set in OBS Studio: ```rtmp://<your_host_ip>/live```. Set key on your choise, e. g. ```test```.

To view a stream open URL in VLC player: ```rtmp://<your_host_ip>/live/<your_key>```
