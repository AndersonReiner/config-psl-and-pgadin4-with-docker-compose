# Iniciando o serviço do PSL e PgAdmin

### 1. Certifique de estar na pasta com os arquivos. 

> `ls`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-24-38.png)

### 2. Execute o comando para o subir os container

> `docker-compose up -d`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-26-40.png)

### 3. Verfique se os container estão executando

> `docker ps`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-27-05.png)


# Conctando ao PgAdmin


### 1. Abra o navegador e digite 

> `localhosta:5050`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-28-46.png)

### 2. Entre com o email e a senha definica no arquivo .yaml

> `EMAIL: reiner.anderson@gmail.com`

> `SENHA: superseguro`


![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-29-11.png)


# Conctando o PgAdmin ao PSl

### 1. Adicione um novo banco

clique em add new server

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-29-33.png)

### 2. adicione um um nome para o novo banco

> `EXEMPLO: postgreSql`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-30-32.png)


### 3. Preecha os campos com as informações contidas no arquivo .yaml

OBSERVAÇÃO: No campo abaixo 
> `HOST NAME/ADDRES`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-32-19.png)