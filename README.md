The program is a local SOCKS proxy server.

[ByeDPI project](https://github.com/hufrea/byedpi)

## Instructions

```bash
git clone https://github.com/anton-savenchuk/byedpi-docker
cd byedpi-docker
```

**Docker**

```bash
docker build . -t byedpi
docker run --rm -p 127.0.0.1:1080:1080 --volume ./list.txt:/list.txt \
    --name byedpi -d byedpi \
    --hosts list.txt \
    -s1 -q1 -Y -Ar -s5 -o1+s -At -f-1 -r1+s -As -s1 -o1 +s -s-1 -An
```

**Docker compose**

```bash
docker compose up --build
```

**Use socks5 proxy server**

```
socks5://127.0.0.1:1080
```
