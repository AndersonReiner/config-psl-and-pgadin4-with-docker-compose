# Iniciando o serviço do PSL e PgAdmin no Docker

### 1. Certifique de estar com o arquivo.yaml na pasta. 

> `ls`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-24-38.png)

### 2. Execute o comando para o subir os container

Certfique-se de estar com o docker compose instalado na sua máquina!

> `docker-compose up -d`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-26-40.png)

### 3. Verfique se os container estão executando

> `docker ps`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-27-05.png)


# Conctando ao PgAdmin


### 1. Abra o navegador e digite 

> `localhosta:5050`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-28-46.png)

### 2. Entre com o email e a senha definido no arquivo .yaml

> `EMAIL: reiner.anderson@gmail.com`

> `SENHA: superseguro`


![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-29-11.png)


# Conctando o PgAdmin ao PSl

### 1. Adicione um novo banco

clique em add new server

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-29-33.png)

### 2. adicione um um nome para o novo banco

> `EXEMPLO: postgreSQL`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-30-32.png)



#  3. Preecha os campos com as informações contidas no arquivo .yaml

> `HOST NAME/ADDRES: postgres_service`

> `PORT: 5432 `

> `MAINTENANCE/DATABASE: postgres`

> `USERNAME: aluno `

> `PASSWORD: superseguro `



![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2020-32-19.png)


Salve as configurações e teste a conexão, se não conseguir procure novamente pelas informações no arquivo .yaml, se o problema persistir tente fazer isso em outra maquina, o docker compose pose estar salvando algum tipo de cache, reinstalar o docker poderia ser uma opção em ultimos casos.



## Instrução de onde localizar as informações necessarias para preencher os campos acima.


### 1. Para preencher o campo `HOST NAME/ADDRES` você deve colocar o nome do serviço como na imagem acima ou o ip do serviço

Você pode localizar ele na linha 4 da imagem abaixo, que mostra trecho do arquivo.yaml

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2021-00-36.png)


ou pode colocar o IpAddress, para isso basta rodar um comando no terminal `docker inspect <nome_do_container>`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-17%2021-08-43.png)

procure pelo `IPAddress`

![Texto Alternativo da Imagem](img/Captura%20de%20tela%20de%202024-03-18%2006-39-46.png)


### Se você chegou até o fim é porque deu certo e não desistiu, é hora de programar!!!
