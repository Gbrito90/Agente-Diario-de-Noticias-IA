# 📚 Pipeline RAG do Guardião IA

## Visão Geral

O Guardião IA usa RAG para responder perguntas com base em documentos corporativos autorizados.

Em vez de depender apenas do conhecimento interno do LLM, o sistema recupera trechos relevantes dos documentos e usa esse contexto para gerar respostas.

## Pipeline

```text
Upload
↓
Extração
↓
Limpeza
↓
Chunking
↓
Embeddings
↓
Vetorização
↓
Indexação
↓
Busca Semântica
↓
Resposta com Evidências
```

## Configuração Atual

- Modelo de embedding: `text-embedding-3-small`
- Estratégia de chunking: aproximadamente 1.200 caracteres com overlap
- Recuperação: busca semântica em chunks indexados
- Evidência: documento, chunk e score de similaridade

## Snapshot Atual

| Métrica | Valor |
|---|---:|
| Documentos indexados | 11 |
| Texto extraído | 35.622 caracteres |
| Chunks | 39 |
| Embeddings | 39 |
| Cobertura | 100% |

## Mitigação de Alucinação

O sistema reduz alucinações com contexto recuperado, citações, score de confiança, risco de alucinação, especialistas e revisão humana.
