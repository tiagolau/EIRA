# PRD — Aplicativo EIRA

**Versao:** 1.0
**Data:** 2026-03-20
**Status:** Rascunho

---

## 1. Resumo Executivo

O aplicativo EIRA e uma plataforma mobile/web que combina **controle financeiro pessoal**, **acompanhamento de investimentos imobiliarios** e um **agente de IA** para orientacao continua. O objetivo e criar um relacionamento duradouro com o cliente, mantendo-o informado, engajado e avancando na jornada de construcao patrimonial pelo Metodo EIRA.

### Missao do Produto

> Ajudar o cliente a construir seus sonhos para uma melhor qualidade de vida, continuamente.

### Problema

- Clientes de consorcio perdem engajamento apos a compra da carta
- Falta visibilidade sobre o progresso do investimento vs. alternativas (renda fixa)
- Controle financeiro pessoal e feito em planilhas ou apps genericos sem conexao com a estrategia imobiliaria
- Informacoes sobre mercado imobiliario e financeiro sao dispersas e genericas

### Solucao

Um app que centraliza: financas pessoais, acompanhamento do consorcio, simulacoes do Metodo EIRA, conteudo relevante e um agente de IA que conhece a situacao financeira do cliente e o orienta proativamente.

---

## 2. Usuarios-Alvo

### Persona 1: Investidor Iniciante
- 25-40 anos, renda R$3k-8k/mes
- Quer sair do aluguel ou ter primeiro imovel
- Pouco conhecimento sobre consorcio
- Precisa de educacao financeira e controle de gastos

### Persona 2: Investidor em Crescimento
- 30-50 anos, renda R$8k-20k/mes
- Ja tem 1-2 imoveis, quer multiplicar patrimonio
- Conhece consorcio basico, precisa das estrategias avancadas
- Busca otimizar rendimento e acelerar contemplacao

### Persona 3: Investidor com Capital
- 35-60 anos, renda R$20k+/mes ou capital acumulado
- Tem capital para lance e/ou compra a vista
- Quer maximizar retorno usando alavancagem via consorcio
- Precisa de simulacoes sofisticadas e acompanhamento proximo

---

## 3. Funcionalidades

### 3.1 Controle Financeiro Pessoal

**Objetivo:** Dar ao cliente visao clara da saude financeira para que possa investir com seguranca.

| Funcionalidade | Descricao | Prioridade |
|----------------|-----------|------------|
| Registro de receitas/despesas | Entrada manual e categorizada | P0 |
| Categorias personalizaveis | Moradia, alimentacao, transporte, lazer, investimentos | P0 |
| Dashboard mensal | Visao consolidada de entradas, saidas e saldo | P0 |
| Metas de economia | Definir meta mensal de economia para investir | P1 |
| Importacao de extrato bancario | Via Open Finance ou upload de OFX/CSV | P2 |
| Recorrencias | Cadastro de despesas e receitas fixas | P1 |
| Alerta de gastos | Notificacao quando ultrapassar limites por categoria | P1 |

### 3.2 Painel de Investimentos EIRA

**Objetivo:** Acompanhar todos os consorcios, imoveis e investimentos do cliente em um so lugar.

| Funcionalidade | Descricao | Prioridade |
|----------------|-----------|------------|
| Cadastro de cartas de consorcio | Valor, parcela, tipo (cheia/meia), administradora, grupo | P0 |
| Status da carta | Ativa, contemplada, quitada, cancelada | P0 |
| Evolucao do credito | Grafico mostrando credito corrigido pelo INCC vs. total pago | P0 |
| Comparativo vs. renda fixa | Grafico lado a lado: consorcio vs. se tivesse aplicado | P0 |
| Acompanhamento de imoveis | Imoveis comprados/construidos, valor estimado, renda de aluguel | P1 |
| Projecao patrimonial | Simulacao de quanto o patrimonio crescera nos proximos 5/10/20 anos | P1 |
| Historico de assembleias | Registro de resultados de sorteio e lances | P1 |
| Patrimonio total | Soma de todos ativos: imoveis + creditos + aplicacoes | P0 |

### 3.3 Simulador do Metodo EIRA

**Objetivo:** Permitir que o cliente (e o vendedor) simule cenarios antes de investir.

| Funcionalidade | Descricao | Prioridade |
|----------------|-----------|------------|
| Simulador de carta | Dado valor da parcela, mostra opcoes de carta (cheia e meia) | P0 |
| Simulador de contemplacao | Compara cenarios: sorteio, lance embutido, lance embutido + livre | P0 |
| Simulador de alavancagem | Mostra poder de compra real vs. capital investido | P0 |
| Simulador de ciclo | Projecao do Crescimento 100%: quantos imoveis em X anos | P1 |
| Simulador de levantamento de capital | Calcula quanto pode levantar com imoveis existentes | P1 |
| Comparativo personalizado | Consorcio vs. financiamento vs. compra a vista vs. renda fixa | P1 |
| Exportar simulacao em PDF | Para apresentar ao cliente ou compartilhar | P2 |

### 3.4 Agente de IA (EIRA AI)

**Objetivo:** Ser o consultor financeiro pessoal do cliente, disponivel 24/7.

| Funcionalidade | Descricao | Prioridade |
|----------------|-----------|------------|
| Chat conversacional | Interface de chat para tirar duvidas sobre financas e investimentos | P0 |
| Contexto financeiro do cliente | IA tem acesso ao perfil, financas e investimentos do usuario | P0 |
| Recomendacoes proativas | Sugerir acoes baseadas na situacao atual (ex: "voce tem R$X sobrando, que tal aumentar o lance?") | P1 |
| Explicacao do Metodo EIRA | Responder duvidas sobre os 6 caminhos e estrategias | P0 |
| Simulacoes via conversa | Cliente pede simulacao no chat e IA retorna cenarios | P1 |
| Alertas inteligentes | "Sua assembleia e amanha", "Seu credito ja corrigiu X%", "Hora de revisar seu orcamento" | P1 |
| Educacao financeira | IA sugere conteudos e explica conceitos sob demanda | P1 |
| Analise de oportunidades | IA avalia se uma oportunidade de compra/construcao faz sentido para o perfil do cliente | P2 |

**Modelo de IA:** Claude (Anthropic) via API, com contexto persistente por usuario.

### 3.5 Feed de Conteudo e Noticias

**Objetivo:** Manter o cliente informado e engajado com conteudo relevante.

| Funcionalidade | Descricao | Prioridade |
|----------------|-----------|------------|
| Feed de noticias | Noticias sobre mercado imobiliario, economia, INCC, Selic, consorcio | P0 |
| Conteudo educacional | Artigos e videos sobre educacao financeira e investimento imobiliario | P1 |
| Atualizacoes EIRA | Novos empreendimentos, oportunidades de compra na planta | P1 |
| Notificacoes push | Alertas de noticias relevantes e atualizacoes de investimentos | P1 |
| Personalizacao do feed | Conteudo filtrado por interesses e perfil do cliente | P2 |
| Newsletter semanal | Resumo semanal enviado por email/push | P2 |

### 3.6 Area do Vendedor (Painel Interno)

**Objetivo:** Ferramentas para o time comercial usar o Metodo EIRA nas vendas.

| Funcionalidade | Descricao | Prioridade |
|----------------|-----------|------------|
| Simulador de venda | Dado o orcamento do cliente, gera proposta com melhor estrategia | P0 |
| Gerador de proposta | PDF com simulacao personalizada para enviar ao cliente | P1 |
| CRM basico | Cadastro de leads e acompanhamento de pipeline | P2 |
| Dashboard de comissoes | Acompanhar vendas e comissoes | P2 |

---

## 4. Arquitetura de Alto Nivel

```
+---------------------+       +---------------------+
|   App Mobile/Web    |       |   Painel Vendedor   |
|   (React Native /   |       |   (Next.js Web)     |
|    Next.js PWA)     |       |                     |
+----------+----------+       +----------+----------+
           |                             |
           +-------------+---------------+
                         |
              +----------+----------+
              |     API Gateway     |
              |     (REST/tRPC)     |
              +----------+----------+
                         |
        +----------------+----------------+
        |                |                |
+-------+------+ +------+-------+ +------+-------+
|  Auth &      | |  Core API    | |  EIRA AI     |
|  Users       | |  (Financas,  | |  Agent       |
|  Service     | |  Consorcios, | |  (Claude API)|
|              | |  Simulacoes) | |              |
+--------------+ +--------------+ +--------------+
        |                |                |
        +----------------+----------------+
                         |
              +----------+----------+
              |     PostgreSQL      |
              |     + Redis Cache   |
              +---------------------+
```

### Stack Sugerida

| Camada | Tecnologia | Justificativa |
|--------|-----------|---------------|
| Mobile | React Native (Expo) | Multiplataforma, ecossistema maduro |
| Web | Next.js 15 (App Router) | SSR, performance, PWA |
| API | Node.js + tRPC ou REST | Type-safe, rapido de desenvolver |
| Banco de dados | PostgreSQL | Robusto, relacional, bom para financas |
| Cache | Redis | Sessoes, cache de simulacoes |
| Auth | Clerk ou Auth.js | Autenticacao pronta, social login |
| IA | Claude API (Anthropic) | Melhor modelo para conversacao e raciocinio financeiro |
| Conteudo/CMS | Strapi ou Payload CMS | Feed de noticias e conteudo educacional |
| Notificacoes | OneSignal ou Firebase Cloud Messaging | Push notifications |
| Hospedagem | Vercel (web) + Railway/Render (API) | Deploy simples, escalavel |
| Monitoramento | Sentry + PostHog | Erros + analytics |

---

## 5. Modelo de Dados (Entidades Principais)

```
User
  - id, name, email, phone, cpf
  - role: client | seller | admin
  - profile: income, patrimony, objectives

FinancialEntry
  - id, user_id, type: income | expense
  - amount, category, date, description
  - recurring: boolean, recurrence_rule

ConsortiumCard
  - id, user_id
  - credit_value, installment_type: full | half
  - monthly_installment, administrator, group_number
  - status: active | contemplated | settled | cancelled
  - purchase_date, contemplation_date
  - embedded_bid_pct, free_bid_amount
  - incc_rate, annual_correction

Property
  - id, user_id, consortium_card_id (nullable)
  - type: apartment | house | land | commercial
  - address, estimated_value, purchase_value
  - rental_income, status: owned | under_construction | sold

Simulation
  - id, user_id
  - type: card | contemplation | leverage | cycle | capital_raise
  - parameters: JSON
  - results: JSON
  - created_at

ChatMessage
  - id, user_id, session_id
  - role: user | assistant
  - content, created_at

NewsArticle
  - id, title, summary, content, category
  - source_url, image_url
  - published_at, tags

AssemblyResult
  - id, consortium_card_id
  - date, drawn_number, bid_winner_amount
  - user_was_drawn: boolean
```

---

## 6. Fluxos Principais

### 6.1 Onboarding do Cliente

```
1. Download do app / acesso web
2. Cadastro (nome, email, telefone)
3. Questionario inicial:
   - Renda mensal
   - Despesas estimadas
   - Patrimonio atual (imoveis, investimentos)
   - Objetivo: primeiro imovel / renda de aluguel / multiplicar patrimonio
   - Quanto pode investir por mes
4. IA analisa perfil e sugere caminho EIRA ideal
5. Cliente acessa dashboard personalizado
```

### 6.2 Simulacao de Investimento

```
1. Cliente informa quanto pode pagar por mes
2. Sistema calcula opcoes de carta (cheia e meia)
3. Mostra cenarios de contemplacao (sorteio, lances)
4. Compara com renda fixa no mesmo periodo
5. Mostra projecao patrimonial em 5/10/20 anos
6. Cliente pode salvar simulacao ou compartilhar
```

### 6.3 Interacao com IA

```
1. Cliente abre chat
2. IA carrega contexto: perfil, financas, consorcios, imoveis
3. Cliente faz pergunta ou pede orientacao
4. IA responde com base no Metodo EIRA e dados do cliente
5. Se relevante, IA sugere simulacao ou acao especifica
6. Historico de conversa persistido para continuidade
```

### 6.4 Controle Financeiro Mensal

```
1. Cliente registra receitas e despesas (ou importa extrato)
2. Dashboard mostra: ganhou X, gastou Y, sobrou Z
3. Sistema compara com meta de economia
4. IA envia insight: "Voce economizou R$X este mes.
   Com esse valor, poderia adquirir uma carta de R$Yk na meia parcela."
5. Cliente acompanha evolucao mes a mes
```

---

## 7. Metricas de Sucesso

| Metrica | Meta (6 meses) | Meta (12 meses) |
|---------|----------------|-----------------|
| Usuarios cadastrados | 500 | 2.000 |
| Usuarios ativos mensais (MAU) | 60% dos cadastrados | 50% dos cadastrados |
| Simulacoes realizadas | 1.000 | 5.000 |
| Interacoes com IA/mes | 3 por usuario ativo | 5 por usuario ativo |
| Retencao D30 | 40% | 50% |
| NPS | >40 | >50 |
| Cartas vendidas via app | 50 | 300 |

---

## 8. Fases de Desenvolvimento

### Fase 1 — MVP (8-12 semanas)

**Foco:** Valor central com minimo esforco.

- Controle financeiro basico (receitas, despesas, dashboard)
- Cadastro e acompanhamento de cartas de consorcio
- Simulador de carta (parcela -> opcoes)
- Comparativo consorcio vs. renda fixa
- Chat com agente de IA (contexto basico)
- Feed de noticias (curadoria manual inicial)
- Auth + perfil do usuario

**Entregavel:** App web (PWA) funcional para primeiros clientes.

### Fase 2 — Engajamento (4-8 semanas apos MVP)

- App mobile (React Native)
- Simulador completo (todos os cenarios)
- IA com contexto financeiro do cliente
- Notificacoes push (assembleias, alertas, insights)
- Metas de economia e alertas de gastos
- Conteudo educacional estruturado
- Projecao patrimonial

### Fase 3 — Escala (8-12 semanas apos Fase 2)

- Open Finance (importacao de extrato)
- Area do vendedor com simulador de venda
- Gerador de proposta em PDF
- IA proativa (recomendacoes sem pedido)
- Personalizacao do feed
- CRM basico para vendedores
- Dashboard de comissoes

### Fase 4 — Ecossistema (continuo)

- Integracao com administradoras de consorcio (APIs)
- Marketplace de imoveis/empreendimentos da construtora
- Comunidade de investidores EIRA
- Gamificacao (niveis de patrimonio, conquistas)
- Relatorios fiscais (IR)

---

## 9. Riscos e Mitigacoes

| Risco | Impacto | Mitigacao |
|-------|---------|-----------|
| Cliente nao engaja apos compra da carta | Alto | IA proativa + conteudo relevante + gamificacao |
| Premissas financeiras mudam (INCC, Selic) | Medio | Parametros configuraveis, simulador atualizado |
| Regulacao sobre consultoria financeira | Alto | Disclaimers claros: app e educacional, nao e consultoria regulada |
| Complexidade do MVP | Medio | Foco brutal no essencial, iterar rapido |
| Custo da IA por usuario | Medio | Cache de respostas comuns, limites de uso no free tier |
| Seguranca de dados financeiros | Alto | Criptografia, LGPD compliance, audit trail |

---

## 10. Monetizacao (Futuro)

| Modelo | Descricao |
|--------|-----------|
| Gratuito para clientes EIRA | Quem tem carta vendida pelo time EIRA usa gratis |
| Freemium | Controle financeiro gratis, simulador avancado e IA no plano pago |
| Comissao de venda | App gera leads qualificados que convertem em vendas de consorcio |
| Parcerias | Construtoras pagam para listar empreendimentos no app |

---

## 11. Consideracoes Legais

- **LGPD:** Consentimento explicito para coleta de dados financeiros. Direito de exclusao.
- **Regulacao financeira:** O app NAO e uma plataforma de investimentos regulada. E uma ferramenta de educacao e controle financeiro. Disclaimers em todas as simulacoes.
- **Termos de uso:** Simulacoes sao estimativas baseadas em premissas. Valores reais podem variar.
