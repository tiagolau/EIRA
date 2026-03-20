# 001 — Estruturacao do Metodo EIRA e PRD do Aplicativo

**Data:** 2026-03-20
**Status:** aceito

## Contexto

O projeto EIRA possuia apenas um documento Word com estrategias brutas de alavancagem patrimonial via consorcio. Era necessario transformar isso em uma metodologia estruturada e definir o produto digital que dara suporte ao relacionamento com o cliente.

## Decisao

1. **Metodologia EIRA** foi formalizada como um framework com 4 pilares (Estrategia, Investimento, Rendimento, Aceleracao) e 6 caminhos de investimento, desde consorcio puro ate ciclo de multiplicacao patrimonial.

2. **PRD do aplicativo** foi criado com foco em: controle financeiro pessoal, painel de investimentos, simulador do metodo, agente de IA conversacional e feed de conteudo. Dividido em 4 fases de desenvolvimento.

3. **Stack sugerida:** React Native (Expo) + Next.js + Node.js + PostgreSQL + Claude API para o agente de IA.

## Alternativas Consideradas

- **Apenas planilha/PDF:** Rejeitado pois nao gera relacionamento continuo com o cliente
- **App so de consorcio:** Rejeitado pois o diferencial e o controle financeiro integrado com a estrategia
- **Sem IA:** Rejeitado pois o agente de IA e o principal diferencial de engajamento

## Consequencias

- O Metodo EIRA agora tem documentacao formal que pode ser usada para treinamento de vendedores e comunicacao com clientes
- O PRD serve como guia para desenvolvimento do MVP
- Proximos passos: definir wireframes, escolher stack final, iniciar desenvolvimento do MVP (Fase 1)
