# EIRA — Estrategia Imobiliaria de Rendimento Acelerado

## Sobre o Projeto

Plataforma de investimento imobiliario que combina controle financeiro pessoal, acompanhamento de consorcios e agente de IA para orientacao continua do cliente.

## Documentacao

- Metodologia: `docs/metodologia/METODO-EIRA.md`
- PRD do aplicativo: `docs/PRD.md`
- Decisoes arquiteturais: `docs/decisions/`

## Stack (planejada)

- Mobile: React Native (Expo)
- Web: Next.js 15 (App Router, PWA)
- API: Node.js + tRPC
- Banco: PostgreSQL + Redis
- IA: Claude API (Anthropic)
- Auth: Clerk ou Auth.js

## Contexto de Negocio

- A EIRA conecta investidores a oportunidades imobiliarias (consorcio, compra na planta, construcao)
- O cliente tem construtora/incorporadora que usa os recursos dos investidores
- O app e o canal de relacionamento continuo com o cliente
- Foco em educacao financeira + acompanhamento de investimentos
