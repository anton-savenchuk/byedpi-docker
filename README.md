[ByeDPI project](https://github.com/hufrea/byedpi)

## Instructions

```bash
git clone https://github.com/anton-savenchuk/byedpi-docker
cd byedpi-docker
```

**Docker**

```bash
docker build . -t byedpi
docker run --rm -p 127.0.0.1:1080:1080 --name byedpi byedpi --split 1 --oob 1 --fake 1 --ttl 1 -A torst --tlsrec 1+sni --debug 1 --auto=none
```

**Docker compose**

```bash
docker compose up --build
```

**Use socks5 proxy server**

```
socks5://127.0.0.1:1080
```
