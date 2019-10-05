## nmap

## Build

```
docker build -t nmap .
docker tag nmap michaeljdennis/nmap:latest
docker push michaeljdennis/nmap:latest
```

## Run

```
docker run --rm -it michaeljdennis/nmap google.com
```
