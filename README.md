# 💸 FinChat - App de Organização de Finanças Pessoais com Vibe Coding

PRD (Product Requirements Document) refinado com o Microsoft Copilot:

```markdown
# PRD — Finanças Pessoais por Conversa (Resumo Simplificado)

## Visão Geral
App de **organização financeira via conversa**, substituindo planilhas e formulários por interação em linguagem natural com um agente financeiro virtual.

---

## Problema
- Apps atuais exigem entrada manual e são pouco intuitivos.  
- Alta taxa de abandono, especialmente entre iniciantes.  
- Usuários precisam de uma ferramenta que **entenda sua realidade**.

---

## Público-Alvo
- **Principal:** Jovens profissionais iniciando vida financeira (ex.: Camila, 27 anos).  
- **Secundários:** Autônomos, casais com renda compartilhada, estudantes universitários.

---

## Funcionalidades-Chave
1. **Registro de Gastos por Conversa**  
   - Ex.: “Paguei 120 reais de luz”  
   - Confirmação + sugestão de categoria.

2. **Classificação Automática**  
   - Categorias padrão: Alimentação, Transporte, Moradia, Saúde, Lazer, Vestuário, Educação, Contas, Outros.  
   - Aprendizado contínuo e personalização.

3. **Metas Financeiras**  
   - Definição em linguagem natural.  
   - Progresso visual + alertas e sugestões.

4. **Agente Financeiro (IA)**  
   - Responde perguntas (“quanto gastei em transporte?”).  
   - Identifica padrões e sugere cortes.  
   - Tom educativo e acolhedor.

5. **Relatórios Simples**  
   - Resumo mensal, evolução de gastos, comparativos.  
   - Gráficos acessíveis por texto/voz e compartilháveis.

---

## Design e Acessibilidade
- Baseado em **Design Universal** e **WCAG 2.1 AA**.  
- Suporte a texto, voz, leitura de tela.  
- Contraste adequado, modo escuro, zoom até 200%.  
- Área de toque mínima 44×44 px.  
- Mensagens claras e sem jargões.  
- Compatibilidade com VoiceOver (iOS) e TalkBack (Android).  
- Funcionalidade básica disponível offline.

---

## Arquitetura de Telas
- **Onboarding** (boas-vindas, renda, primeira meta).  
- **Home (Chat)** — tela principal com resumo do mês.  
- **Transações** — lista, detalhe, busca.  
- **Metas** — progresso e criação.  
- **Relatórios** — gráficos e comparativos.  
- **Configurações** — perfil, categorias, notificações, acessibilidade.

---

## Requisitos Técnicos
- **Plataformas:** Android (≥8.0), iOS (≥14), Web PWA (pós-MVP).  
- **Infra:** IA conversacional, SQLite + nuvem, autenticação Google/Apple, notificações push, modo offline.  
- **Segurança:** TLS 1.3, AES-256, LGPD, exportação/exclusão de dados.

---

## MVP e Validação
- **Cronograma (8 semanas):**  
  - Sprints 1–2: Onboarding, autenticação, chat.  
  - Sprints 3–4: Registro e classificação.  
  - Sprints 5–6: Metas e resumo mensal.  
  - Sprints 7–8: Acessibilidade e testes.  

- **Critérios de saída:**  
  - Registro em <15s.  
  - Classificação ≥80% acerto.  
  - Acessibilidade aprovada.  
  - Onboarding concluído por ≥85%.  

- **KPIs:**  
  - Registro via chat ≥80%.  
  - Retenção D7 ≥40%, D30 ≥25%.  
  - NPS ≥45.  
  - Precisão ≥85%.

---

## Fora do Escopo
- Conexão com bancos (Open Finance).  
- Controle de investimentos.  
- Gestão compartilhada.  
- Exportação para Excel/Sheets.  
- Suporte a múltiplas moedas.  
- Versão web completa no MVP.

---

## Glossário
- **Agente Financeiro:** IA que conduz conversas e orienta.  
- **Transação:** Registro de entrada/saída financeira.  
- **Meta:** Objetivo financeiro com valor e prazo.  
- **Classificação automática:** Categorização feita pela IA.  
- **WCAG:** Diretrizes internacionais de acessibilidade.  
- **LGPD:** Lei brasileira de proteção de dados.  
- **MVP:** Versão mínima viável para testes.

```

Interações com o Lovable

> Crie um app de finanças pessoais baseado no seguinte Product Requirements Document: {PRD}
> O app está repetindo o onboarding sem a pessoa usuária pedir (bug gerado pelo Lovable).
> Crie 3 screenshots para apresentar o app.

Resultado final no Lovable: https://finchat-dialogue.lovable.app

<img width="550" height="1040" alt="image" src="https://github.com/user-attachments/assets/b348da91-eec2-418c-b62f-6a11596d7800" />
<img width="550" height="1040" alt="image" src="https://github.com/user-attachments/assets/18978792-47db-45f1-92a9-6614cf8bd3f3" />
<img width="550" height="1040" alt="image" src="https://github.com/user-attachments/assets/4bb0b4d7-b810-4016-a5cb-0f58174377b7" />

# FinChat — Resumo de funcionalidades

O **FinChat** é um app mobile-first de finanças pessoais com foco em registrar receitas, despesas e metas por meio de uma experiência conversacional simples.

## Funcionalidades principais

### Chat financeiro
- Registro de despesas e receitas por linguagem natural.
- Exemplos:
  - “gastei R$45 no almoço”
  - “recebi R$3.200 de salário”
- Identificação automática de valor, tipo da transação e categoria.
- Confirmação visual da transação registrada.
- Chips rápidos para ações como ver relatório, criar meta e receber dica do dia.

### Dashboard mensal
- Visão resumida do mês atual.
- Cards com:
  - Receitas
  - Despesas
  - Saldo
- Lista das últimas transações.
- Insights automáticos com base nos maiores gastos.
- Seletor de mês para navegar entre períodos.

### Relatórios
- Gráfico de distribuição de gastos por categoria.
- Evolução diária dos gastos no mês.
- Métricas como total gasto e maior categoria.
- Lista de transações agrupadas por data.
- Filtros por categoria.
- Botão de exportação em PDF com aviso de “Em breve”.

### Metas financeiras
- Criação e acompanhamento de metas.
- Cards com:
  - Emoji
  - Título da meta
  - Valor atual
  - Valor alvo
  - Progresso percentual
  - Prazo
- Ação para adicionar valor à meta.
- Animação de comemoração ao concluir uma meta.
- Opção para excluir metas.

### Onboarding
- Fluxo inicial simples em etapas.
- Coleta de:
  - Nome
  - Renda mensal aproximada
  - Categorias mais frequentes
  - Objetivo financeiro
- Demonstração de como registrar gastos pelo chat.
- O onboarding aparece apenas na primeira experiência do usuário.

## Experiência e design

- Interface limpa, minimalista e mobile-first.
- Layout otimizado para viewport de 390px.
- Navegação inferior com quatro abas:
  - Chat
  - Dashboard
  - Relatórios
  - Metas
- Design com destaque em verde/teal.
- Componentes acessíveis com bons tamanhos de toque.
- Suporte a preferências de redução de movimento.

## Escopo técnico

- App feito com React, TypeScript, Tailwind CSS e shadcn/ui.
- Dados mockados e persistidos localmente.
- Sem login, backend, banco de dados ou APIs reais.
- Processamento de linguagem natural simulado com regras e padrões simples.

## Reflexão

### O que funcionou bem? 
   Usar o Microsoft Copilot para refazer o PRD com mais detalhes precisos fez o Lovable criar em pouco tempo o app de acordo com o que foi pedido no PRD.
### O que não funcionou como o esperado?
   O Lovable fez o app com um erro que estava reiniciando o processo de onboarding. Mas foi possível corrigir esse com um prompt no próprio Lovable.
### O que aprendeu sobre conversar com IAs?
   Aprendi que usando a linguagem natural e prompts detalhados com descrições precisas, é possível colocar em prática o vibe coding para criar softwares funcionais de uma maneira muito mais fácil.

