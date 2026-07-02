# 🏢 Arquitetura Multi-Tenant

## Visão Geral

O Guardião IA foi pensado como um SaaS Multi-Tenant, onde cada empresa opera em um workspace isolado.

Cada workspace possui seus próprios usuários, documentos, agentes, ferramentas, logs e configurações.

## Isolamento

Cada workspace isola:

- Usuários
- Documentos
- Agentes
- Chunks
- Embeddings
- Logs
- Configurações

## Papéis

- Admin
- Editor
- Viewer
- Auditor

## Fluxo Seguro

```text
Usuário
↓
Autenticação
↓
Validação do Workspace
↓
Validação de Permissão
↓
Busca Vetorial no Workspace
↓
Resposta Auditável
```

## Objetivo

Evitar vazamento de dados entre empresas e permitir uso corporativo seguro.
