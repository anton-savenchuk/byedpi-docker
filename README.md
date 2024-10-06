[ByeDPI project](https://github.com/hufrea/byedpi)

## Instructions

**Docker**

```bash
docker build . -t byedpi
docker run --rm -p 127.0.0.1:1080:1080 --name byedpi byedpi --split 1 --oob 1 --fake 1 --ttl 1 -A torst --tlsrec 1+sni --debug 1 --auto=none
```

**Use socks5 proxy server**

```
socks5://127.0.0.1:1080
```
