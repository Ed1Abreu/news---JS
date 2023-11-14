
# Site de notícias em Docker

## Iniciando o Docker

### Imagem

```
news---js-nginx
```

### 1. Instalação do Docker Desktop

#### Realizar a instalação do [Docker Desktop](https://www.docker.com/products/docker-desktop/)

### 2. Com o projeto aberto digite o seguinte comando no terminal

```
docker pull nginx
```

### 3. Iniciar aplicação
#### Depois Digite o seguinte comando no terminal aberto no repositório

```
docker run --hostname=5bdf5bc2c76e --env=PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin --env=NGINX_VERSION=1.25.3 --env=PKG_RELEASE=1 --env=NJS_VERSION=0.8.2 --network=news---js_noticia -p 30001:80 --label='com.docker.compose.config-hash=c7e8817c26fec3369164437f6c69427c89be9e21ca1bd29e381149983eed3370' --label='com.docker.compose.container-number=1' --label='com.docker.compose.depends_on=' --label='com.docker.compose.image=sha256:4cdac6f2dafbb5f35266054d3f46e9e12c22069154bd0d3bd80b113cdfc011b7' --label='com.docker.compose.oneoff=False' --label='com.docker.compose.project=news---js' --label='com.docker.compose.project.config_files=C:\Users\edvan\OneDrive\Documentos\news---JS\compose.yaml' --label='com.docker.compose.project.working_dir=C:\Users\edvan\OneDrive\Documentos\news---JS' --label='com.docker.compose.service=proxy' --label='com.docker.compose.version=2.23.0' --label='maintainer=NGINX Docker Maintainers <docker-maint@nginx.com>' --runtime=runc -d noticia-nginx
```
