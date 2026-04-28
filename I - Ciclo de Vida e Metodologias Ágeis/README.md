## Eixo 1: Ciclo de Vida e Metodologias Ágeis

Nesta pasta encontram-se os artefatos de auditoria referentes ao ciclo de vida de desenvolvimento, metodologias ágeis adotadas e decisões arquiteturais do projeto ScrapeGraphAI, fundamentados na análise de evidências digitais do repositório.

## Conteúdo da Auditoria

* **1_camada_abstracao/:** Diretório contendo os arquivos `base_graph.py` e `fetch_node.py`, que comprovam materialmente o uso de abstração para isolar a lógica principal do sistema das APIs de terceiros.
* **2_provedores_ia/:** Diretório contendo os arquivos `deepseek.py` e `nvidia.py`, evidenciando a estratégia técnica do projeto para combater a dependência de um único fornecedor.
* **3_exemplos_flexibilidade/:** Diretório contendo scripts comparativos (`smart_scraper_lite_ollama.py` e `smart_scraper_lite_openai.py`) e instruções (`readme.md`), provando a facilidade de adaptação da ferramenta.

## Resumo dos Achados

* O projeto adota um modelo **semi-ágil orientado por demanda**, assemelhando-se ao Kanban, em que as *Issues* atuam como o núcleo do planejamento, evidenciando um fluxo descentralizado sem o uso estruturado de *Milestones*.
* O ciclo de publicações (*Releases*) segue o padrão de **Continuous Delivery** (Entrega Contínua), com atualizações incrementais e ágeis liberadas assim que o código estabiliza, sem um calendário fixo.
* O risco técnico crítico de dependência de APIs externas (como a OpenAI) é fortemente mitigado por uma **camada de abstração**, garantindo que as mudanças de terceiros não quebrem o motor principal do projeto.
* O sistema possui **alta flexibilidade arquitetural**, permitindo ao usuário transitar rapidamente entre modelos pagos na nuvem e modelos gratuitos rodando localmente (Ollama) com a alteração de apenas uma linha de configuração.



**Auditor Responsável:** Christian Will Silva Santos Nunes
