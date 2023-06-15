<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>



# executado em desenvolvimento

1. Clonar o repositorio
2. Executar

``` 
 npm install
```
3. Ter Nest Cli instalado
```
npm i -g @nestjs/cli
```

4. Levantar a base de dados
```
docker-compose up
```

5. Clonar o arquivo __.env.template e renomear a .env

6. Chamar as variaveis de retorno definadas no .env

7. Executar a aplicacao

8. Reconstruir a base de dados com a semente
```
http://localhost:3000/api/v2/seed
```

## Stack usdado
* MongoDB
* Nest

# Production Build
1. Criar o arquivo ```.env.pro```
2. Chamar as variaveis retorno do prod
3. Criar uma nova imagem
```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```