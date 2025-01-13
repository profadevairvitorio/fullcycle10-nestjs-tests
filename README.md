![Imersão Full Stack && Full Cycle](https://events-fullcycle.s3.amazonaws.com/events-fullcycle/static/site/img/grupo_4417.png)

## Sobre o repositório
Esse repositório contém o código-fonte ministrado nas aulas:

Durante estas 3 aulas, mostramos como:

## Rodar a aplicação

```bash
docker compose up 
```

```bash
docker compose -f docker-compose.prod.yaml up 
```

Entre no container do Nest.js para levantar o servidor WEB:

```bash
docker compose exec app bash
npm run start:dev

docker compose -f docker-compose.prod.yaml exec app bash
npm run start:dev
```



Use o arquivo `api.http` para testar a publicação usando a extensão Rest Client do VSCode ou outra ferramenta para brincar com o HTTP.
