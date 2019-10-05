## awscli

## Build

```
docker build --build-arg AWS_DEFAULT_REGION=us-east-1 --build-arg AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID> --build-arg AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY> -t awscli .
```

Or if the build args are already set as environment variables in your local system:

```
docker build --build-arg AWS_DEFAULT_REGION --build-arg AWS_ACCESS_KEY_ID --build-arg AWS_SECRET_ACCESS_KEY -t awscli .
```

# Run

```
docker run --rm -it awscli
```
