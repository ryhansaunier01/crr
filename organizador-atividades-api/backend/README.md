# Organizador de Atividades — API

API REST para gerenciamento de atividades, construída com Fastify e MySQL.

**Autor:** Ryhan Saunier

## Recursos

- Listagem de atividades com busca por texto e filtro por status
- Criação de atividades com prazo opcional
- Atualização parcial (título, prazo e status de conclusão)
- Remoção de atividades

## Como executar

```bash
npm install
npm run dev
```

Configure as variáveis de ambiente em um arquivo `.env` (host, porta, usuário, senha e nome do banco de dados). O banco e a tabela são criados automaticamente na inicialização, caso ainda não existam.

## Endpoints principais

| Método | Rota              | Descrição                          |
|--------|-------------------|-------------------------------------|
| GET    | `/api/tasks`       | Lista atividades (com filtros)      |
| POST   | `/api/tasks`       | Cria uma nova atividade             |
| PATCH  | `/api/tasks/:id`   | Atualiza uma atividade existente    |
| DELETE | `/api/tasks/:id`   | Remove uma atividade                |

Exemplos de requisições estão disponíveis em `rotas.http`.
