# Análise de aderência ao perfil e portfólio

## Síntese do perfil considerado

A coletânea foi desenhada para uma trajetória de transição e consolidação em dados: experiência extensa em relacionamento, negócios e contexto bancário; atuação atual como Analista de Dados; formação em Administração e Computação; especializações em Analytics, Engenharia de Dados e IA; e projetos práticos que atravessam análise, pipelines, cloud, ML e aplicações com LLMs.

Essa combinação sugere um diferencial útil: conectar a necessidade do negócio à implementação técnica e à comunicação do resultado. Por isso, as Skills não ficam restritas a código. Incluem definição de problema, granularidade e indicadores, validação, governança, operação e documentação.

## Mapeamento indicativo para projetos compartilhados

O mapeamento abaixo se baseia nas descrições dos projetos compartilhadas nas conversas e na memória de trabalho. Não representa uma auditoria atual do código, dos testes ou do estado dos repositórios.

| Projeto ou linha de trabalho | Skills mais relacionadas | O que a coletânea ajuda a sistematizar |
|---|---|---|
| `indicadores-bcb` e projetos de indicadores econômicos | `data-project-scoping`, `data-pipeline-engineering`, `data-analytics-eda`, `sql-data-analysis`, `technical-data-documentation` | Contratos de fonte, atualização idempotente, reconciliação, explicação de indicadores e entrega de relatórios. |
| `pipeline-credito-inteligente-aws` e projetos de crédito | `multicloud-data-architecture`, `data-pipeline-engineering`, `data-quality-governance`, `ml-model-development` | Integração entre ingestão, processamento, modelagem, segurança e consumo; separação entre demonstração e decisão financeira operacional. |
| `pipeline-e2e-vendas`, `pipeline-vendas-ecommerce` e ETLs | `data-pipeline-engineering`, `sql-data-analysis`, `data-quality-governance`, `data-analytics-eda` | Batch e incremental, modelo dimensional, regras de qualidade, testes e indicadores de negócio. |
| `etl-ipca-boi-gordo`, `pipeline-dados-financeiros` e B3/Spark/Delta | `databricks-lakehouse`, `data-pipeline-engineering`, `sql-data-analysis`, `technical-data-documentation` | Camadas Bronze/Silver/Gold, transformações distribuídas, validação de séries temporais e documentação executável. |
| `corporate-knowledge-assistant` e assistente RAG financeiro local | `rag-knowledge-assistant`, `data-quality-governance`, `ai-agent-engineering`, `technical-data-documentation` | Evidências e citações, avaliação de recuperação, tratamento de lacunas, segurança de fontes e limites de resposta. |
| `ai-code-review-plataform`, `trustops-ai-plataform` e STEH | `ai-data-code-review`, `ai-agent-engineering`, `data-quality-governance`, `technical-data-documentation` | Revisões sustentadas por evidências, desenho de ferramentas e políticas, supervisão humana, rastreabilidade e testes. |
| `mlops-breast-cancer`, `calculo-ml`, `copa_predict` e recomendação | `ml-model-development`, `data-analytics-eda`, `data-pipeline-engineering`, `technical-data-documentation` | Baselines, prevenção de leakage, métricas adequadas, análise de erro, reprodutibilidade e explicação de resultados. |
| `InvestIQ` e analytics para negócios | `data-project-scoping`, `data-analytics-eda`, `sql-data-analysis`, `ml-model-development` | Tradução de necessidade de usuário em indicador, hipótese, análise e funcionalidade orientada a decisão. |

## Decisões de desenho das Skills

1. **A análise começa pela pergunta de negócio.** A experiência de negócios e atendimento é aproveitada para definir usuários, decisão e indicador antes de escolher tecnologia.
2. **A engenharia inclui operação.** Pipelines são tratados com incrementalidade, idempotência, recuperação, qualidade e observabilidade, temas recorrentes nos projetos de Lakehouse, APIs, batch e streaming.
3. **A ciência de dados exige avaliação honesta.** As instruções enfatizam baseline, split correto, leakage, análise de erro e limitações, em vez de focar apenas no algoritmo.
4. **Sistemas com LLM precisam de evidência e controle.** As Skills de RAG e agentes cobrem fontes, avaliação, permissões, prompt injection, limites e aprovação humana.
5. **Governança e privacidade atravessam o fluxo.** O contexto bancário pede exemplos sintéticos, minimização, controle de acesso e evidências rastreáveis; nenhum conteúdo interno da CAIXA deve ser colocado em repositório público.
6. **Documentação é parte do produto.** README, diagramas, ADRs, execução e limitações ajudam a tornar os projetos reproduzíveis e demonstrar decisões de engenharia.

## Como evoluir a coletânea

- Adicione uma regra específica de projeto somente depois de validar que ela é recorrente e correta.
- Vincule cada Skill a testes ou exemplos reais sintéticos quando uma regra depender de código.
- Crie uma Skill dedicada a MLOps ou monitoramento quando houver um fluxo recorrente bem definido de deploy, registro, monitoramento e retreino.
- Mantenha regras que se aplicam a todos os pedidos em `AGENTS.md`; deixe nas Skills os procedimentos especializados.
- Revise comandos e APIs cloud/Databricks contra a versão efetivamente usada no projeto.
