# Sistema de Inteligência Artificial Autônoma

## 🚀 Visão Geral
Este projeto implementa uma arquitetura de IA baseada em múltiplos agentes autônomos capazes de planejar, executar código dinâmico, avaliar resultados e aprender de forma contínua.

## 🛠️ Arquitetura do Sistema
O sistema opera em um ciclo evolutivo composto por:
- **Agente Autônomo:** Define metas e objetivos de aprendizado.
- **Orquestrador:** Coordena o fluxo entre planejamento e execução.
- **Executor:** Roda código Python gerado dinamicamente para testes e tarefas.
- **Auto-Evoluidor:** Módulo de aprendizado que extrai padrões e atualiza a memória interna.
- **Busca Web:** Enriquecimento de contexto através de fontes externas.

## 📊 Fluxo de Execução
```mermaid
flowchart TD
A[Agente Autônomo] --> B[Orquestrador]
B --> C[Busca Web]
B --> D[Executor]
D --> E[Crítico]
E --> F{Aprovado?}
F -->|Sim| G[Auto-Evoluidor]
F -->|Não| B
G --> H[Memória]
H --> A

