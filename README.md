# AI Skills — Fabio Estevam

Coletânea de Skills reutilizáveis para projetos de análise, ciência e engenharia de dados e IA. A estrutura usa o formato `SKILL.md` e fica em `.agents/skills`, para ser versionada junto a um repositório e consultada por agentes compatíveis.

## Perfil que orienta esta coletânea

As Skills foram organizadas para apoiar uma trajetória que combina experiência bancária e foco no cliente com análise de dados, formação em Administração e Computação, especializações em dados/Analytics/IA e projetos práticos de pipelines, Lakehouse, indicadores econômicos, ML, RAG e agentes. As instruções favorecem soluções explicáveis, reprodutíveis, documentadas e orientadas a requisitos de negócio.

## Catálogo

| Skill | Quando usar |
|---|---|
| `data-project-scoping` | Transformar uma necessidade em escopo e critérios de aceite. |
| `data-analytics-eda` | Explorar datasets, verificar qualidade e levantar achados. |
| `sql-data-analysis` | Escrever ou revisar SQL analítico e validar indicadores. |
| `data-pipeline-engineering` | Projetar pipelines batch, incrementais ou streaming. |
| `databricks-lakehouse` | Construir soluções Databricks, Spark e Delta. |
| `data-quality-governance` | Definir contratos, qualidade, catálogo, linhagem e acesso. |
| `multicloud-data-architecture` | Comparar e desenhar arquiteturas Azure, AWS e GCP. |
| `ml-model-development` | Estruturar e avaliar soluções de machine learning. |
| `rag-knowledge-assistant` | Projetar e avaliar assistentes RAG com evidências. |
| `ai-agent-engineering` | Projetar agentes, ferramentas, políticas e HITL. |
| `ai-data-code-review` | Revisar código de dados, ML, RAG e agentes. |
| `technical-data-documentation` | Criar README, arquitetura, ADRs e manuais. |

## Como usar em um repositório

1. Copie a pasta `.agents/skills` para a raiz do repositório que contém o projeto.
2. Abra o repositório com um agente que reconheça Agent Skills.
3. Peça a tarefa diretamente ou mencione a Skill pelo nome, por exemplo:

> Use `data-pipeline-engineering` para revisar este pipeline. Verifique incrementalidade, idempotência, qualidade, quarentena e reprocessamento. Aponte evidências e lacunas.

> Use `rag-knowledge-assistant` para elaborar um plano de avaliação. Inclua perguntas sem resposta, referências esperadas, métricas de recuperação e testes de segurança.

> Use `databricks-lakehouse` para revisar este notebook. Confirme a versão/API disponível antes de sugerir alterações e explique o papel de Bronze, Silver e Gold.

4. Confira o diff e a resposta do agente. Atualize a Skill se uma correção recorrente ou regra de projeto estiver faltando.

## Organização e compatibilidade

`SKILL.md` contém metadados YAML (`name` e `description`) e instruções em Markdown. O nome deve corresponder à pasta. As Skills desta coletânea estão em `.agents/skills`; confira a documentação da ferramenta/versão do agente utilizada, pois os locais de descoberta podem variar. Para instruções que se aplicam a toda tarefa de codificação, mantenha regras gerais em `AGENTS.md`; use Skills para procedimentos especializados acionados quando pertinentes.

## Princípios e limites

- Priorize evidências do código, dos dados e dos testes; declare hipóteses e incertezas.
- Use dados públicos, sintéticos ou explicitamente autorizados em exemplos.
- Não inclua segredos, dados reais de clientes, documentos internos ou informações proprietárias da CAIXA neste repositório.
- Para serviços de nuvem, preços, legislação e APIs sujeitos a mudança, confirme fontes e versões atuais antes de orientar uma implantação.
- Exemplos didáticos não representam automaticamente uma solução pronta para produção.
- Escolha e inclua uma licença antes de tornar o repositório público, se quiser definir permissões de reutilização.

## Atualização

Comece com uma tarefa real, observe onde a Skill falha ou é ambígua e edite instruções específicas. Mantenha cada Skill focada em um trabalho e mova referências longas para arquivos próprios quando necessário.
