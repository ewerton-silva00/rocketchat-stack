# RocketChat Stack

Siga os passos abaixo para inicializar este ambiente de testes.

**Passo 01:** Crie uma network chamada ```traefik-network```.
```bash
docker network create --driver bridge traefik-network
```

**Passo 02:** Adicione no ```/etc/hosts``` do seu notebook/desktop as entradas de DNS abaixo.
```
127.0.0.1 traefik.meudominio.local
127.0.0.1 chat.meudominio.local
```

**Passo 03:** Execute o arquivo ```docker-compose.yml```.
```bash
docker-compose up --detach
```

**Passo 04:** Acesse os serviços no browser.
```
traefik.meudominio.local
chat.meudominio.local
```

**Observação:** A interface do Traefik está protegida por usuário e senha.
```
User: admin
Password: password
```

Documentações utilizadas para executar esse ambiente:

https://docs.traefik.io/  
https://rocket.chat/docs/installation/docker-containers/docker-compose/  
https://rocket.chat/docs/administrator-guides/setting-up-video-conferencing/  