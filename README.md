# try-traefik

# docker-compose up/down just one container

```bash
docker-compose rm -fsv [yourService]
```


# make cert

- https://zenn.dev/jeffi7/articles/10f7b12d6044ad

## chrome

- https://stackoverflow.com/questions/7580508/getting-chrome-to-accept-self-signed-localhost-certificate
- [chrome://flags/#allow-insecure-localhost](chrome://flags/#allow-insecure-localhost) Set Enable

## docker secret

### Init swarm

```bash
docker swarm init
```

### Create secret files

```bash
docker secret create my_web_crt cert/localhost.crt
docker secret create my_web_key cert/localhost.key
```

### LS secret files

```bash
docker secret ls
```
