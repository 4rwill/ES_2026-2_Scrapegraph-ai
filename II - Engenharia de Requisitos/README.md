# 🔍 Eixo 2: Engenharia de Requisitos (GRE)

Nesta pasta encontram-se os artefatos de auditoria referentes à Gerência de Requisitos (REQM / MPS.BR) do projeto **ScrapeGraphAI**.

## Conteúdo da Auditoria
1. **`matriz_rastreabilidade.csv`**: Planilha contendo o mapeamento bidirecional exato de 3 requisitos auditados no projeto, evidenciando o "Fio de Ariadne" solicitado na disciplina.
2. **`evidencias/`**: Diretório contendo as capturas de tela que comprovam a utilização de *Issue Templates*, debates em *Discussions* (RFC informal) e a amarração entre as Issues e os Pull Requests.

## Resumo dos Achados
* O projeto utiliza **Issue Templates** para forçar a elicitação correta de novos requisitos (Feature Requests).
* A rastreabilidade de código é mantida de forma nativa pelo GitHub, vinculando Issues fechadas a seus respectivos Commits e Pull Requests.
* A gestão de mudanças é automatizada com o uso de bots (`dosubot` e `semantic-release`) para encerrar requisições ociosas (*stale*) e empacotar releases rastreáveis.

## Links Oficiais das Trilhas Auditadas
* **Requisito 1 (Batch API):** [Issue #1036](https://github.com/ScrapeGraphAI/Scrapegraph-ai/issues/1036)
* **Requisito 2 (Timeout):** [Issue #831](https://github.com/ScrapeGraphAI/Scrapegraph-ai/issues/831)
* **Requisito 3 (Amazon Bedrock):** [Issue #633](https://github.com/ScrapeGraphAI/Scrapegraph-ai/issues/633)

---
**Auditor Responsável:** Rian Purificação de Oliveira
