# Make PHP Fast Again

Just test it with compose:
```sh
podman compose up -d

# or

docker compose up -d
```

site:
1. http://localhost:8787 -> PHP CLI builtin server
2. http://localhost:8888 -> PHP FPM + Nginx + Opcache
3. http://localhost:8989 -> PHP FPM + Nginx + Opcache + FastCGI Page Cache

## Result
Macbook Air M2 16GB 512GB
```
PHP CLI Builtin Server    -> 150 RPS
PHP FPM + Nginx + Opcache ->  2K RPS
PHP FPM + Nginx + Opcache -> 13K RPS
```

