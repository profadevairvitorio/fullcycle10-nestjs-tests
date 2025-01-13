![Imersão Full Stack && Full Cycle](https://events-fullcycle.s3.amazonaws.com/events-fullcycle/static/site/img/grupo_4417.png)

Participe gratuitamente: https://imersao.fullcycle.com.br/

## Sobre o repositório
Esse repositório contém o código-fonte ministrado nas aulas:

Durante estas 3 aulas, mostramos como:

* Desenvolver API Rest e testes automatizados (pirâmide de testes) com Nest.js
* Como montar um ambiente de desenvolvimento com Docker no VSCode satisfazendo necessidades como: backup dos banco de dados de dados em volumes, tmpfs para testes, terminal ZSH dentro do container e Remote Container
* Como montar uma esteira de CI/CD (Integração Contínua e Deploy Contínuo) usando Github Action, Github Packages, Artifact Registry e Cloud Run

## Rodar a aplicação

```bash
docker compose up # para levantar a versão de desenvolvimento
```

```bash
docker compose -f docker-compose.prod.yaml up  # para levantar a versão de produção
```

Entre no container do Nest.js para levantar o servidor WEB:

```bash
# versão de desenvolvimento
docker compose exec app bash
npm run start:dev

# versão de produção
docker compose -f docker-compose.prod.yaml exec app bash
npm run start:dev
```



Use o arquivo `api.http` para testar a publicação usando a extensão Rest Client do VSCode ou outra ferramenta para brincar com o HTTP.