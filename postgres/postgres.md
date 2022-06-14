# Ambiente postgres para estudos

A ideia deste projeto consiste na criação de um ambiente para estudos de banco de dados PostgreSQL.


Necessário ter o `docker` e também o `docker-compose` instalado.


Documentação Instalação Docker

https://docs.docker.com/engine/install/

Documentação Instalação Docker-compose

https://docs.docker.com/compose/install/compose-plugin/#installing-compose-on-linux-systems


Versões testadas:
```
Docker version 20.10.17, build 100c701
Docker Compose version v2.6.0
```




## Criação de diretórios:

Criação dos diretórios:
```bash
mkdir -p pgdata pgadmin
```

Configuração de permissão para o diretório pgadmin:
```bash
sudo chown 5050:5050 pgadmin
```


## Subindo o ambiente
```bash
docker-compose up -d
```

## Acessando o pdadmin

Acessar a URL: `http://IP-do-host:8080`


usuário: `user@domain.com`

senha: `postgres`


## Desligando o ambiente
```bash
docker-compose down
```