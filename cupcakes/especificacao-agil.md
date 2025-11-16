# Especificação Ágil — Projeto Loja de Cupcakes (Thiago Nogueira)

## Resumo
Documento consolidado contendo backlog priorizado, critérios de aceite, cronograma iterativo, proposta de SGBD (PostgreSQL), script DDL, estrutura de repositório Git, fluxo de branches, checklist para ciclo de melhoria contínua e template de pedido de feedback aos colegas.

## Mudanças e melhorias aplicadas
- Padronização de IDs e critérios de aceite.
- Inclusão de histórias faltantes (estoque, webhooks de pagamento, logs de auditoria).
- Requisitos não-funcionais mensuráveis (tempo resposta, limites de upload, segurança).
- Proposta SGBD: PostgreSQL.
- Estrutura Git/CI para manter documentação e código no mesmo repositório.

## Backlog (resumido)
Veja o arquivo backlog.csv para o backlog completo com 20 histórias priorizadas e estimadas.

## Cronograma iterativo sugerido (exemplo)
- Sprint 0 (configuração): 1 dia
- Sprint 1 (MVP): 7 dias — cadastro, vitrine, carrinho, checkout (sandbox)
- Sprint 2 (Admin e estoque): 5 dias
- Sprint 3 (Qualidade e entrega): 4 dias
- Buffer e ajustes: 3 dias
Total estimado: 20 dias úteis.

## SGBD sugerido
PostgreSQL (mature, comunidade ativa, compatível com ORMs). Use migrations (Flyway/Alembic/TypeORM).

## Scripts SQL
Arquivo: schema.sql (contém DDL exemplo para users, products, orders, order_items, payments, reviews, audit_logs).

## Repositório Git sugerido
Estrutura proposta:

project-cupcakes/
├─ README.md
├─ .gitignore
├─ app/
├─ web/
├─ infra/
├─ docs/
└─ tests/


Branching: main (produção), develop (integração), feature/<id>-descrição.

## CI/CD
Arquivo: .github/workflows/ci.yml (workflow básico com install/test).

## Processo de feedback
- Enviar solicitação com template.
- Registrar feedback como issues com label feedback.
- Incorporar no backlog.

## Checklist de qualidade
- Histórias com critérios claros
- Testes automatizados
- Migrations versionadas
- Documentação atualizada
- Segurança verificada
