# Project Cupcakes (MVP)

Repositório com estrutura recomendada para o projeto da loja de cupcakes.

## Como rodar (exemplo com Docker Compose)

1. Configure variáveis de ambiente (`.env`)
2. Execute:

docker-compose up --build
3. Rode migrations (ex.: `npx sequelize db:migrate`, `alembic upgrade head`, etc.)
4. Acesse a aplicação em:
- Frontend: `http://localhost:3000`
- Backend/API: `http://localhost:8000`

---

## Estrutura sugerida

project-cupcakes/
├─ README.md
├─ .gitignore
├─ app/
├─ web/


---

## Boas práticas recomendadas

- Usar PostgreSQL para desenvolvimento e produção.
- Manter migrations versionadas e organizadas.
- Criar branches por feature (`feature/<nome>`).
- Criar Pull Requests com descrição clara.
- Evitar commits grandes: preferir commits pequenos e frequentes.
- Sempre atualizar a documentação após cada mudança importante.

---

## Documentação do projeto

- **especificacao-agil.md**: documentação principal.
- **backlog.csv**: histórias de usuário, prioridades e pontos.
- **schema.sql**: DDL para criação do banco PostgreSQL.

---

Qualquer dúvida, fale com o autor do projeto.

├─ infra/
├─ docs/
└─ tests/
