# 🏗️ Arquitetura do Guardião IA

## Visão Geral

O Guardião IA é uma plataforma Enterprise de Document Intelligence criada para permitir que empresas consultem documentos internos com segurança, rastreabilidade e apoio de IA Generativa.

A arquitetura combina RAG, agentes especializados, workspaces, auditoria, avaliação de IA e governança corporativa.

## Fluxo de Alto Nível

```text
Usuário
↓
Autenticação
↓
Workspace
↓
Roteador de Agentes
↓
Especialista de IA
↓
Retriever
↓
Ferramentas Corporativas
↓
LLM
↓
Avaliação RAG
↓
Resposta Auditável
↓
Logs e Analytics
```

## Camadas Principais

1. Camada de Autenticação
2. Camada Multi-Tenant / Workspace
3. Camada de Gestão Documental
4. Camada RAG
5. Camada Multi-Agent
6. Camada de Observabilidade
7. Camada de Governança e Auditoria

## Decisões Arquiteturais

- Responder apenas com base em documentos autorizados.
- Separar dados por workspace.
- Registrar consultas, fontes e métricas.
- Exibir risco de alucinação.
- Permitir avaliação e benchmark do RAG.

## Estado Atual

O projeto já possui login, dashboard, documentos, pipeline RAG, agentes, Explain AI, RAG Evaluation Center e Benchmark Module.
