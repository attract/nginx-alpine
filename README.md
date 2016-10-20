# nginx-alpine

example docker-compose

``` nginx:
        network_mode: "bridge"
        build:
          context: .
          dockerfile: ./nginx/Dockerfile
        restart: always
    volumes:
          - ./nginx/sites/host.conf:/etc/nginx/sites-available/vhost.conf
          - ./nginx/nginx.conf:/etc/nginx/nginx.conf        