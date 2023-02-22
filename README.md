# react_ui_template

## Development

Build the image:

```console
docker build --no-cache -f Dockerfile.dev -t react_ui_template:latest .
```

Run a container:

```console
docker run --rm -it -p 3000:3000/tcp -p 9229:9229/tcp react_ui_template:latest
```

## Production

Build the image:

```console
docker build --no-cache -f Dockerfile.prod -t react_ui_template:latest .
```

Run a container:

```console
docker run --rm -it -p 3000:3000/tcp react_ui_template:latest
```
