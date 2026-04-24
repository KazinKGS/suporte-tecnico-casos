# Caso 03 - Criação de relatório simples no ERP Sankhya via SQL Oracle

## Problema
Necessidade de gerar um relatório simples para visualização de notas fiscais no sistema ERP.

## Diagnóstico
- Identificada a necessidade de consulta direta no banco de dados
- Definidos os campos principais: número da nota, valor e produto

## Solução
Desenvolvida consulta SQL simples no banco Oracle:

```sql
SELECT 
    TGLNOTA.NUMNOTA,
    TGLNOTA.VLRNOTA,
    TGLNOTA.CODPROD
FROM 
    TGLNOTA
