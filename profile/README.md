# Kaikan Cachoeira

Sistema de gestão para uma associação sem fins lucrativos dedicada a preservar a cultura japonesa, mantida inteiramente por voluntários. A associação promove eventos como karaokê, gincanas, bingos e torneios, e durante esses eventos opera uma lanchonete (baiten) para ajudar a cobrir as despesas mensais.

## O problema

Hoje todo o controle financeiro, de estoque e de doações é feito manualmente, no papel ou em planilhas Excel. Isso dificulta:

- o planejamento de compras (não há histórico de vendas por evento);
- a visibilidade sobre sobras de produtos entre eventos;
- saber quanto cada evento efetivamente gerou de lucro;
- rastrear doações recebidas (dinheiro, produtos, materiais) e o "vale" (ficha) dado em agradecimento.

## Escopo do sistema

O foco é o controle **agregado** por evento, não o rastreamento de cada transação individual feita por cada atendente. Principais frentes:

- **Gestão de eventos**: Cadastro, status (planejado / em andamento / encerrado), produtos vendidos, histórico de vendas
- **Gestão de estoque**: Entrada e saída de produtos, sobras entre eventos
- **Controle de doações**: Dinheiro, produtos e materiais, vinculados ao associado doador
- **Relatórios financeiros**: Custo, receita e lucro líquido por evento
- **Dashboards gerenciais**: Indicadores financeiros, de vendas e de estoque

## Repositórios

| Repo | Conteúdo |
|---|---|
| [`kaikan-cachoeira-api`](https://github.com/kaikan-cachoeira/kaikan-cachoeira-api) | API em Java/Spring Boot |
| [`kaikan-cachoeira-web`](https://github.com/kaikan-cachoeira/kaikan-cachoeira-web) | Aplicação web em React/Vite |
| [`kaikan-cachoeira-docs`](https://github.com/kaikan-cachoeira/kaikan-cachoeira-docs) | Padrões de commit, fluxo de branches e contrato de API (`ENDPOINTS.md`) |

## Stack

**Backend:** Java 21, Spring Boot, Spring Data JPA, PostgreSQL, Docker Compose
**Frontend:** React, Vite
**Ferramentas:** Maven, Git/GitHub

Detalhes de setup e como rodar cada parte estão no README de cada repositório.

## Equipe

| Nome | GitHub |
|---|---|
| Marlon de Souza | [@marlonzl7](https://github.com/marlonzl7) |
| Reginaldo de Souza | [@regisdesouza](https://github.com/regisdesouza) |
| Lucas Eiki | [@lucas-eiki](https://github.com/lucas-eiki) |
| Rayza Gomes | [@RayzaDSbr](https://github.com/RayzaDSbr) |
| Gabriela Pereira | [@GabrielaPereiraSantana](https://github.com/GabrielaPereiraSantana) |
| Daniel Foschini | [@D-Foschini](https://github.com/D-Foschini) |

## Fluxo de trabalho

Todos os repositórios seguem o mesmo padrão de branches e commits, documentado em [`kaikan-cachoeira-docs`](https://github.com/kaikan-cachoeira/kaikan-cachoeira-docs):

```
feat/nome-da-feature → dev → main
```
