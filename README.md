# collabora/code without ssl

## Usage

```bash
docker build --tag collabora/nossl .
docker run -itd -p 9980:9980 --name collabora -e username=admin -e password=password collabora/nossl
```

## Docker Compose

```yaml
collabora:
  build: .
  image: collabora/nossl
  restart: always
  environment:
    username: admin
    password: password
  ports:
    - 9980:9980
```


