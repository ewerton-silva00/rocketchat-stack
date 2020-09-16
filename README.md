# RocketChat Stack

Siga os passos abaixo para inicializar este ambiente de testes localmente no seu computador.

**Passo 01:** Adicione no ```/etc/hosts``` do seu notebook/desktop as entradas de DNS abaixo.
```
127.0.0.1 traefik.meudominio.local minio.meudominio.local chat.meudominio.local
```

**Passo 02:** Execute o arquivo ```docker-compose.yml```.
```bash
docker-compose up --detach
```
> Caso queira prender a execução da stack no STDOUT basta executar o comando acima sem o ```detach```.

**Passo 03:** Acesse os serviços no browser.
```
traefik.meudominio.local
minio.meudominio.local
chat.meudominio.local
```

**Observação:** O **Dashboard** do Traefik está protegida por usuário e senha.
```
User: admin
Password: password
```

Documentações utilizadas para executar esse ambiente:

https://docs.traefik.io/
https://docs.min.io/
https://rocket.chat/docs/installation/docker-containers/docker-compose/
https://rocket.chat/docs/administrator-guides/setting-up-video-conferencing/