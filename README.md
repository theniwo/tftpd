# Usage

```
docker run -d \
        --name tftpd \
        --restart unless-stopped \
        -v "tftpd_data:/data" \
        -p 69:69/udp \
        -e PUID=1000 \
        -e PGID=1000 \
        -e TFTP_OPTIONS=--create \
        theniwo/tftpd
```


