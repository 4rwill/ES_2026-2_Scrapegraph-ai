# Relatório de Contribuição Individual e Rastreabilidade de Pesquisa

**Disciplina:** Engenharia de Software  
**Projeto Analisado:** [Scrapegraph-ai](https://github.com/ScrapeGraphAI/Scrapegraph-ai)  
 

## Integrantes:
* ARTHUR SOARES SANTANA (202400051087)
* ARTUR JOSÉ SOARES SANTOS (202400072372)
* ANGELO DE SOUSA MUTTI (202100045555)
* CHRISTIAN WILL SILVA SANTOS NUNES (202400050796)
* EDUARDO FERREIRA BOMFIM FILHO (202400050811)
* EDUARDO CURCINO MONTEIRO FILHO (202400051102)
* IURI MAURICIO MAIA PEREIRA (202400051120)
* RIAN PURIFICAÇÃO DE OLIVEIRA (202400051013)

---

## Detalhamento das Contribuições por Eixo

### 1. Eixo 1 - Ciclo de Vida e Metodologias Ágeis
* **Responsável:** Christian Will
* **O que fez:** Analisou o ciclo de desenvolvimento do projeto, identificando a adoção de um modelo semi-ágil (Kanban) e práticas semelhantes ao *Continuous Delivery*. Avaliou também as estratégias de mitigação de riscos arquiteturais, especificamente o tratamento da dependência de APIs externas de IA através de camadas de abstração.
* **Onde procurou as informações:** A investigação foi conduzida através da observação direta da interface do GitHub do repositório original. Verificou as abas de `Issues`, `Milestones`, `Projects`, o histórico de `Releases` e inspecionou a estrutura do código responsável pela integração com provedores como OpenAI e Anthropic.

### 2. Eixo 2 - Engenharia de Requisitos
* **Responsável:** Rian Purificação
* **O que fez:** Avaliou o alinhamento da gerência de requisitos do projeto com as diretrizes do CMMI (REQM) e MPS.BR. Comprovou a eficácia da rastreabilidade bidirecional (Matriz de Rastreabilidade Dinâmica) auditando o ciclo de vida de três requisitos reais: API em lote da OpenAI, controle sistêmico de *timeout* e suporte ao Amazon Bedrock.
* **Onde procurou as informações:** O aluno mapeou o fluxo de trabalho analisando a aba de `Discussions`, os Issue Templates (formulários de *Feature Request*) e o documento `CONTRIBUTING.md`. Para a auditoria prática, rastreou as conexões nativas do GitHub entre Issues (#1036, #831, #633), Pull Requests (#1039, #636) e os respectivos commits semânticos.

### 3. Eixo 3 - Arquitetura e Modelagem
* **Responsáveis:** Artur José e Eduardo Curcino
* **O que fez:** 
* **Onde procurou as informações:** 

### 4. Eixo 4 - Verificação e Validação
* **Responsável:** Eduardo Ferreira
* **O que fez:** 
* **Onde procurou as informações:** 

### 5. Eixo 5 - Qualidade de Software
* **Responsáveis:** Angelo Mutti e Iuri Maurício
* **O que fez:** Diagnosticou o nível de aderência do projeto aos padrões de Garantia da Qualidade (PPQA/GQA). Identificou as ferramentas de análise estática utilizadas, avaliou o cumprimento do guia de contribuição e levantou como a equipe do projeto gerencia a dívida técnica.
* **Onde procurou as informações:** Foram analisados os arquivos de configuração de ambiente e linting (`pyproject.toml`, `Makefile`), fluxos do GitHub Actions (`test-suite.yml`, `codeql.yml`), regras do `CONTRIBUTING.md` e buscas ativas por marcações de dívida técnica (ex: `TODOs`) em arquivos específicos do código, como `scrapegraphai/integrations/burr_bridge.py`.

### 6. Plano de Melhoria Sugerido
* **Responsável:** Arthur Soares
* **O que fez:** Consolidou os diagnósticos dos eixos anteriores para estruturar um plano estratégico de elevação de maturidade (foco nos Níveis G e F do MPS.BR). Propôs quatro ações técnicas: criação de Dashboard de Monitoramento (GPR), Matriz de Rastreabilidade de Prompts (GRE), refatoração com *Chain of Responsibility* (PJR) e pipeline de testes de regressão de IA (V&V).
* **Onde procurou as informações:** O aluno baseou-se nos relatórios gerados pelos colegas nos Eixos de 1 a 5, cruzando essas lacunas com os guias oficiais do MPS.BR e CMMI. Para as soluções técnicas propostas, buscou referências em padrões de arquitetura de software (*Design Patterns*) e na literatura técnica de testes voltados para Inteligência Artificial (ex: uso do dataset *ScrapeGraphAI-100k*).
