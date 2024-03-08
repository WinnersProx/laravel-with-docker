

## Laravel with Docker & NGINX

Ensure you have docker installed on your system

## How to run the project

1. Building the image

```
docker build . --no-cache -t winnersprox/laravel-with-nginx
```

2. Running the project from the container

```
docker run -p 90:80 --rm winnersprox/laravel-with-nginx
```

3. In order to map volumes we can run it this way

```
docker run -p 90:80 -v __LOCAL_PATH__/laravel-docker-demo/src:/var/www/html/public --rm winnersprox/laravel-with-nginx
```
