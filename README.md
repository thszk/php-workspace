# PHP Workspace

Este Workspace é destinado a servir aplicações web em PHP com banco de dados MySQL.


## Dependências

Para executar este ambiente, você precisará ter o Docker e o Docker Compose instalados em sua máquina.

- [Docker Engine](https://docs.docker.com/engine/install/)

- [Docker Compose](https://docs.docker.com/compose/install/)


## Estrutura

O workspace possui a seguinte estrutura:

```
php-workspace/
├── .webserver/
│   ├── 000-default.conf
│   └── Dockerfile
├── docker-compose.yml
├── README.md
├── projeto-1
├── projeto-2
└── [...]
```

- O diretório `.webserver` contém os arquivos de configurações do servidor web `Apache` e `PHP`.

- O arquivo `docker-compose.yml` configura os containers do `webserver` e do banco de dados `MySQL 8`.

Para adicionar um projeto, basta colocá-lo na raiz do workspace e acessá-lo no navegador. O nome da pasta será usado como path principal, por exemplo, o `projeto-1` é acessado em `http://localhost/projeto-1`.

Essa estrutura proporciona uma experiência semelhante ao XAMPP, mas com a flexibilidade e facilidade de containers.


## Desenvolvendo

Para iniciar o ambiente de desenvolvimento execute o comando na raiz do workspace:

```
docker-compose up -d
```


Para iniciar o ambiente de desenvolvimento execute o comando na raiz do workspace:


```
docker-compose down
```