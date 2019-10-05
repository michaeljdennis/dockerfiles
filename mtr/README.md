## mtr

## Build

```
docker build -t mtr .
docker tag mtr michaeljdennis/mtr:latest
docker push michaeljdennis/mtr:latest
```

## Run

```
docker run --rm -it michaeljdennis/mtr google.com
```
