## GLPI-DOCKER


Este docker-compose foi criado para subir um servidor de GLPI com 02 containers 01 para a aplicação e outro para o Banco de dados.

## Dependências

- Git
- Docker
- Docker-Compose


### Passo a Passo

- Clone o Repositório:

```shellscript

git clone https://github.com/WesllenMatias/glpi-docker.git && cd glpi-docker

```

- Executado o comando acima, deve ser criado um arquivo dentro da pasta do projeto chamado mysql.env, com o conteudo abaixo:

```shellscript

MYSQL_ROOT_PASSWORD=
MYSQL_DATABASE=
MYSQL_USER=
MYSQL_PASSWORD=

```

__Nestas Variaveis devem ser informados respectivamente a senha do root do mysql, o nome do banco para ser usado no GLPI, o usuário do banco de dados e a senha dele.__


- Proximo passo é subir os containers basta executar o comando abaixo:

```docker

docker-compose build -d

```

