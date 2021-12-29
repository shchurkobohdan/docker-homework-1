# Build image 
```shell
docker build -t my-docs .
```

# Run container
```shell
docker run my-docs
```

# Run with binding all ports
```shell
docker run -P my-docs
```

# Run with specific port
```shell
docker run -p 8080:80 my-docs
```

# Run with limits
```shell
docker run --cpus 1 --memory 10m -p 8080:80 my-docs
```
