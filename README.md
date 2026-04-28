Aqui está o README com a escrita aprimorada, mantendo exatamente a mesma estrutura:

---

# 💸 FinChat - App de Organização de Finanças Pessoais com Vibe Coding

PRD (Product Requirements Document) refinado com o Microsoft Copilot:

```markdown
# PRD — Finanças Pessoais por Conversa (Resumo Simplificado)

## Visão Geral
App de **organização financeira via conversa**, que substitui planilhas e formulários por interação em linguagem natural com um agente financeiro virtual.

---

## Problema
- Apps atuais exigem entrada manual de dados e oferecem pouca intuitividade.
- Alta taxa de abandono, especialmente entre usuários iniciantes.
- Usuários precisam de uma ferramenta que **compreenda sua realidade financeira**.

---

## Público-Alvo
- **Principal:** Jovens profissionais que estão iniciando sua vida financeira (ex.: Camila, 27 anos).
- **Secundários:** Autônomos, casais com renda compartilhada e estudantes universitários.

---

## Funcionalidades-Chave
1. **Registro de Gastos por Conversa**
   - Ex.: "Paguei 120 reais de luz"
   - Confirmação imediata da transação com sugestão de categoria.

2. **Classificação Automática**
   - Categorias padrão: Alimentação, Transporte, Moradia, Saúde, Lazer, Vestuário, Educação, Contas e Outros.
   - Aprendizado contínuo com personalização baseada no comportamento do usuário.

3. **Metas Financeiras**
   - Definição de objetivos em linguagem natural.
   - Acompanhamento visual do progresso com alertas e sugestões contextuais.

4. **Agente Financeiro (IA)**
   - Responde perguntas sobre gastos ("quanto gastei em transporte?").
   - Identifica padrões de consumo e sugere oportunidades de corte.
   - Tom educativo e acolhedor em todas as interações.

5. **Relatórios Simples**
   - Resumo mensal, evolução de gastos e comparativos por período.
   - Gráficos acessíveis por texto ou voz, com opção de compartilhamento.

---

## Design e Acessibilidade
- Baseado em **Design Universal** e nas diretrizes **WCAG 2.1 AA**.
- Suporte a interação por texto, voz e leitores de tela.
- Contraste adequado, modo escuro e zoom de até 200%.
- Área de toque mínima de 44×44 px em todos os elementos interativos.
- Mensagens claras, objetivas e sem jargões técnicos.
- Compatibilidade com VoiceOver (iOS) e TalkBack (Android).
- Funcionalidade básica disponível mesmo sem conexão à internet (modo offline).

---

## Arquitetura de Telas
- **Onboarding** — boas-vindas, coleta de renda e definição da primeira meta.
- **Home (Chat)** — tela principal com resumo do mês e campo de conversa.
- **Transações** — lista completa, visualização de detalhes e busca.
- **Metas** — acompanhamento de progresso e criação de novos objetivos.
- **Relatórios** — gráficos analíticos e comparativos históricos.
- **Configurações** — perfil, categorias, notificações e preferências de acessibilidade.

---

## Requisitos Técnicos
- **Plataformas:** Android (≥8.0), iOS (≥14), Web PWA (pós-MVP).
- **Infra:** IA conversacional, SQLite com sincronização em nuvem, autenticação via Google/Apple, notificações push e modo offline.
- **Segurança:** TLS 1.3, AES-256, conformidade com a LGPD, além de exportação e exclusão de dados sob demanda.

---

## MVP e Validação
- **Cronograma (8 semanas):**
  - Sprints 1–2: Onboarding, autenticação e chat.
  - Sprints 3–4: Registro e classificação de transações.
  - Sprints 5–6: Metas financeiras e resumo mensal.
  - Sprints 7–8: Acessibilidade e testes de qualidade.

- **Critérios de saída:**
  - Registro de transação concluído em menos de 15 segundos.
  - Taxa de acerto na classificação automática igual ou superior a 80%.
  - Conformidade com os requisitos de acessibilidade aprovada.
  - Taxa de conclusão do onboarding igual ou superior a 85%.

- **KPIs:**
  - Registro via chat em ≥80% das sessões.
  - Retenção D7 ≥40% e D30 ≥25%.
  - NPS ≥45.
  - Precisão da classificação ≥85%.

---

## Fora do Escopo
- Conexão com instituições financeiras via Open Finance.
- Controle e acompanhamento de investimentos.
- Gestão financeira compartilhada entre múltiplos usuários.
- Exportação de dados para Excel ou Google Sheets.
- Suporte a múltiplas moedas.
- Versão web completa no MVP.

---

## Glossário
- **Agente Financeiro:** IA responsável por conduzir conversas e orientar o usuário.
- **Transação:** Registro de entrada ou saída financeira.
- **Meta:** Objetivo financeiro com valor definido e prazo determinado.
- **Classificação automática:** Categorização de transações realizada pela IA.
- **WCAG:** Diretrizes internacionais de acessibilidade para conteúdo web.
- **LGPD:** Lei Geral de Proteção de Dados Pessoais, legislação brasileira vigente.
- **MVP:** Versão mínima viável do produto, destinada a testes e validação.
```

Interações com o Lovable

- Crie um app de finanças pessoais baseado no seguinte Product Requirements Document: {PRD}
- O app está reiniciando o onboarding sem que a pessoa usuária tenha solicitado (bug gerado pelo Lovable).
- Crie 3 screenshots para apresentar o app.

Resultado final no Lovable: https://finchat-dialogue.lovable.app

<img width="550" height="1040" alt="image" src="https://github.com/user-attachments/assets/b348da91-eec2-418c-b62f-6a11596d7800" />
<img width="550" height="1040" alt="image" src="https://github.com/user-attachments/assets/18978792-47db-45f1-92a9-6614cf8bd3f3" />
<img width="550" height="1040" alt="image" src="https://github.com/user-attachments/assets/4bb0b4d7-b810-4016-a5cb-0f58174377b7" />

# FinChat — Resumo de funcionalidades

O **FinChat** é um app mobile-first de finanças pessoais que simplifica o registro de receitas, despesas e metas por meio de uma experiência conversacional intuitiva.

## Funcionalidades principais

### Chat financeiro
- Registro de despesas e receitas utilizando linguagem natural.
- Exemplos:
  - "gastei R$45 no almoço"
  - "recebi R$3.200 de salário"
- Identificação automática de valor, tipo de transação e categoria correspondente.
- Confirmação visual imediata após cada transação registrada.
- Chips de ações rápidas para ver relatório, criar meta e receber a dica do dia.

### Dashboard mensal
- Visão consolidada do mês em andamento.
- Cards com indicadores de:
  - Receitas totais
  - Despesas totais
  - Saldo disponível
- Lista das transações mais recentes.
- Insights automáticos com base nos maiores gastos do período.
- Seletor de mês para navegar entre períodos anteriores.

### Relatórios
- Gráfico de distribuição de gastos por categoria.
- Linha de evolução diária dos gastos ao longo do mês.
- Métricas resumidas como total gasto e categoria de maior impacto.
- Lista de transações agrupadas por data.
- Filtros de visualização por categoria.
- Botão de exportação em PDF (funcionalidade marcada como "Em breve").

### Metas financeiras
- Criação e acompanhamento de objetivos financeiros personalizados.
- Cards com:
  - Emoji identificador
  - Título da meta
  - Valor atual acumulado
  - Valor alvo definido
  - Percentual de progresso
  - Data limite
- Ação para adicionar valores à meta a qualquer momento.
- Animação de comemoração ao atingir uma meta.
- Opção para excluir metas existentes.

### Onboarding
- Fluxo inicial dividido em etapas progressivas e simples.
- Coleta de informações essenciais:
  - Nome do usuário
  - Renda mensal aproximada
  - Categorias de gasto mais frequentes
  - Objetivo financeiro principal
- Demonstração prática de como registrar gastos pelo chat.
- Exibido exclusivamente na primeira utilização do app.

## Experiência e design

- Interface limpa, minimalista e otimizada para uso em dispositivos móveis.
- Layout projetado para viewport de 390px de largura.
- Navegação inferior com quatro abas principais:
  - Chat
  - Dashboard
  - Relatórios
  - Metas
- Identidade visual com destaque em verde/teal.
- Componentes acessíveis com áreas de toque adequadas.
- Suporte nativo a preferências de redução de movimento.

## Escopo técnico

- App desenvolvido com React, TypeScript, Tailwind CSS e shadcn/ui.
- Dados mockados e persistidos localmente no dispositivo.
- Sem autenticação, backend, banco de dados remoto ou integração com APIs externas.
- Processamento de linguagem natural simulado por meio de regras e padrões simples.

## Reflexão

### O que funcionou bem?
Utilizar o Microsoft Copilot para detalhar e refinar o PRD permitiu que o Lovable gerasse o app em pouco tempo, com alto alinhamento ao que foi especificado.

### O que não funcionou como o esperado?
O Lovable produziu um bug que reiniciava o fluxo de onboarding inadvertidamente. O problema foi corrigido com sucesso por meio de um prompt diretamente no Lovable.

### O que aprendeu sobre conversar com IAs?
Aprendi que, com linguagem natural e prompts detalhados contendo descrições precisas, é possível praticar o vibe coding e criar softwares funcionais de forma muito mais acessível e eficiente.

---
