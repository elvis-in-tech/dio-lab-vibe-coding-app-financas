# 💸 FinChat - App de Organização de Finanças Pessoais com Vibe Coding

Aprenda a **criar soluções com IA** de forma criativa, guiando ferramentas como o **Claude** e o **Lovable** com uma comunicação simples e natural. O foco é desenvolver o conceito de um **App de Organização de Finanças Pessoais**, mas, acima de tudo, aprender o **jeito Vibe de programar com IA**.

## ✨ O que é Vibe Coding

**Vibe Coding** é uma forma leve e criativa de desenvolver com IA, baseada em **conversas naturais e bem estruturadas**. Você não precisa escrever código linha por linha. Em vez disso, aprende a **guiar a IA** descrevendo suas ideias de forma clara, com **intenção e contexto**. Em outras palavras:

> Você mostra a vibe da sua ideia e a IA transforma em solução (ou em um caminho para ela).

## 🎯 Desafio

Problema: Muitas pessoas não conseguem manter um controle financeiro porque os aplicativos exigem muita entrada de dados manual, e a criação de orçamentos é vista como algo tedioso. 

Precisamos de uma solução que permita **controlar as finanças por meio de uma conversa simples**, com **agentes de IA** capazes de criar **planos de economia personalizados e automatizados**. Você deve utilizar as ideias de **Vibe Coding** e **MVP (Produto Mínimo Viável)** para desenvolver o **conceito de um aplicativo** que resolva o problema citado.

> [!IMPORTANT]
> Você **não precisa construir o código**! O foco está em **usar a IA como sua parceira criativa**, transformando boas ideias e prompts em conceitos funcionais que simulam um produto real.

## 🪄 Etapas do Desafio

### 1. Saber o que Pedir é a Chave! Otimize seus Prompts!

Antes de pedir para a IA "criar um app", é importante definir com clareza o que você quer construir e por quê. Para isso, você vai criar um **PRD (Product Requirements Document)** simplificado, uma especificação que serve como _briefing_ para a IA entender sua ideia.

Um bom PRD deve descrever o problema, quem será beneficiado, as principais funcionalidades e o que você espera que a IA entregue. Use o modelo abaixo como ponto de partida e adapte conforme o seu estilo:

```txt
# PRD — FinChat

**Versão:** 1.2 · **Fase:** MVP · **Horizonte:** 0–6 meses

---

## Problema

Apps de finanças pessoais têm alta taxa de abandono por excesso de fricção na entrada de dados. Formulários longos, categorias manuais e interfaces densas afastam usuários iniciantes antes que o hábito se forme.

---

## Solução

Aplicativo mobile de controle financeiro baseado em conversa. O usuário digita livremente — "gastei R$45 no almoço" — e o app classifica, registra e atualiza os relatórios automaticamente. Um agente financeiro sugere ajustes com base nos padrões reais de gasto.

---

## Personas

| Persona | Perfil | Dor principal |
|---|---|---|
| Laura, 24 — Iniciante | Primeiro emprego, usuária de WhatsApp | Nunca conseguiu manter um hábito de controle |
| Ricardo, 34 — Em transição | Já tentou planilhas e outros apps | Considera as ferramentas complicadas demais |
| Paula, 29 — Freelancer | Renda variável | Sem visibilidade do saldo disponível no mês |

---

## Objetivos

| # | Meta | Indicador |
|---|---|---|
| 1 | Reduzir tempo de lançamento | < 10 segundos por transação |
| 2 | Reter usuários ativos | ≥ 40% no D30 |
| 3 | Validar experiência conversacional | ≥ 70% preferem ao app anterior |
| 4 | Estimular criação de metas | ≥ 50% dos usuários com ao menos 1 meta |

---

## Funcionalidades do MVP

| Funcionalidade | Prioridade | Critério de aceite |
|---|---|---|
| Registro via chat em linguagem natural | Crítica | ≥ 85% de acurácia na interpretação; resposta em < 2s |
| Classificação automática de transações | Crítica | ≥ 80% de acurácia; correção com 1 toque |
| Metas financeiras | Alta | Meta criada em até 3 turnos; progresso em tempo real |
| Agente com dicas proativas | Alta | ≥ 1 insight/semana após 7 dias de dados |
| Relatórios por período e categoria | Média | Acessível em 1 clique; gráficos de rosca e linha |
| Onboarding conversacional | Crítica | ≤ 5 perguntas; concluído em < 3 min; ≥ 75% de conclusão |

**Fora do escopo do MVP:** integração bancária, OCR de comprovantes, multimoeda, versão web, gamificação.

---

## Arquitetura de telas

```
Tab 1 — Chat        Campo de texto livre + chips de atalho + histórico de mensagens
Tab 2 — Dashboard   Saldo do mês + progresso de metas + últimas transações + insight
Tab 3 — Relatórios  Gráfico de rosca + gráfico de linha + lista filtrável
Tab 4 — Metas       Lista de metas + FAB para criar nova meta
Onboarding          Fluxo de 5 etapas (apenas no primeiro acesso)
```

---

## Design Universal — WCAG 2.1 AA

O app deve ser navegável por completo com VoiceOver (iOS) e TalkBack (Android).

**Contraste e cor**
- Texto: contraste mínimo 4,5:1. Componentes de UI: mínimo 3:1.
- Cor nunca é o único indicador: receitas usam verde + ícone + prefixo "+"; despesas usam vermelho + ícone + prefixo "−".
- Badges de categoria exibem sempre ícone + rótulo de texto.

**Toque e espaçamento**
- Área mínima de toque: 44×44px. Espaçamento entre alvos adjacentes: 8px.
- Itens de lista: ≥ 52px de altura. Barra de abas: ≥ 56px. Botão FAB: 56×56px.
- Nenhuma funcionalidade depende exclusivamente de swipe.

**Tipografia**
- Unidades rem em todos os tamanhos — nunca px fixo no elemento raiz.
- Tamanho mínimo: 0,875rem. Altura de linha: 1,5 para corpo, 1,3 para títulos.
- Caixa normal em toda a interface — sem ALL CAPS.

**Marcação semântica**
- Elementos semânticos: `<main>`, `<nav>`, `<section aria-label>`, `<header>`.
- Todo botão com apenas ícone deve ter `aria-label`.
- Ícones decorativos devem ter `aria-hidden="true"`.
- Gráficos devem ter `aria-label` com resumo textual dos dados.
- Inputs sempre associados a um elemento `<label>`.

**Movimento**
- Respeitar `prefers-reduced-motion`: remover confete, substituir dots animados por "Digitando...", trocar slides por aparecimento instantâneo.

**Prevenção de erros**
- Ações destrutivas exigem confirmação com descrição do que será removido.
- Mensagens de erro específicas: não "Erro ao salvar", mas "Verifique se o valor foi preenchido corretamente (ex: 45,90)".
- Toda transação pode ser editada ou excluída a qualquer momento.

**Linguagem**
- Português simples, sem jargão financeiro sem explicação.
- Mensagens do agente: curtas, amigáveis e não-julgamentais.

---

## Métricas de sucesso

| Métrica | Meta |
|---|---|
| Retenção D7 | ≥ 60% |
| Retenção D30 | ≥ 40% |
| NPS (após 30 dias) | ≥ 45 |
| Acurácia do NLP | ≥ 85% |
| Conclusão do onboarding | ≥ 75% |
| Usuários com ≥ 1 meta criada | ≥ 50% |

---

## Plano de validação

**Semanas 1–2:** entrevistas com 15 usuários + teste de usabilidade em protótipo Figma.

**Semanas 3–6:** beta fechado com 50 usuários, coleta de logs de NLP e teste A/B de chips vs. campo livre. Auditoria de acessibilidade com VoiceOver e TalkBack.

**Semanas 7–12:** abertura para lista de espera (até 500 usuários), monitoramento das métricas e decisão de go/no-go para V1.5.

---

## Riscos principais

| Risco | Impacto | Mitigação |
|---|---|---|
| NLP com acurácia < 80% | Alto | Confirmação obrigatória quando confiança for baixa |
| Usuário não cria hábito | Médio | Notificações contextuais + streak de dias |
| Custo de API de IA elevado | Médio | Cache de classificações + modelo local para categorização |
| Componentes inacessíveis no lançamento | Médio | axe-core no CI + teste manual por release |

---

## Roadmap

| Fase | Prazo | Destaque |
|---|---|---|
| MVP | 0–3 meses | Chat, classificação, metas, relatórios, onboarding |
| V1.5 | 3–5 meses | OCR de comprovantes, recorrências, exportação PDF |
| V2.0 | 5–8 meses | Open Finance, análise preditiva, modo família, web |
| Futuro | 8+ meses | Investimentos, gamificação, marketplace |

---

*Revisão a cada sprint de 2 semanas durante o desenvolvimento do MVP.*
```

> [!TIP]
> Pense no PRD/Prompt como “o briefing que a IA precisa para entender sua vibe”. Portanto, quanto mais claro e intencional for o texto, mais próximas do ideal serão as respostas da IA.

### 2. Explorando o Lovable na Prática

Com seu PRD pronto e revisado, é hora de colocar a IA em ação. Abra o Lovable, cole seu prompt completo e peça o plano inicial do MVP do seu aplicativo. Como o plano gratuito limita você a 5 interações por dia, seja estratégico:
- Faça perguntas diretas e construtivas, como “crie o fluxo de telas com base nas funcionalidades listadas” ou “gere uma versão resumida do plano de MVP”;
- Priorize clareza nas instruções para aproveitar ao máximo cada resposta;

Durante essa etapa, você pode orientar a IA para três entregas principais:
1. Agente Financeiro: defina o comportamento e o tom de voz de um consultor financeiro pessoal, alinhado ao público e objetivo do app.
2. Fluxo de Telas: peça à IA para gerar o fluxo conceitual de telas com base nas funcionalidades descritas no PRD, simulando a interação por conversa.
3. Plano de MVP: solicite um resumo das 5 funcionalidades principais, dos recursos necessários e um plano de validação inicial (como medir se o app cumpre seu propósito).

> [!TIP]
> Se preferir, você pode fazer tudo com o **Copilot**. O importante é exercitar a habilidade de transformar intenções em instruções claras e testar os limites da IA como parceira criativa.

### 3. Entregando o Desafio na DIO

Finalize seu projeto criando um **repositório no GitHub** (pode ser um **fork** deste).  
No README do seu repositório, inclua:

- Seu **prompt final** (PRD);  
- Prints ou pequenos vídeos das interações com a IA;  
- Um resumo do que o seu **App de Finanças Pessoais** faz;  
- Uma breve **reflexão sobre o processo**:
  - O que funcionou bem?  
  - O que não funcionou como o esperado?  
  - O que aprendeu sobre conversar com IAs?

> [!TIP]
> Publique seu repositório e compartilhe o link na plataforma da DIO! Sua entrega é a prova de que você domina o raciocínio de Vibe Coding, mesmo sem escrever uma única linha de código.

## 💬 Conclusão

Vibe Coding é sobre clareza, curiosidade e criatividade, não sobre perfeição técnica. O verdadeiro objetivo aqui é aprender a pensar junto com a IA, transformando ideias em conceitos reais e enxergando a tecnologia como uma extensão do seu raciocínio criativo. Cada interação é um experimento, quanto mais clara for sua intenção, mais surpreendente será o resultado.
