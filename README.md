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


- Um resumo do que o seu **App de Finanças Pessoais** faz;  
- Uma breve **reflexão sobre o processo**:
  - O que funcionou bem?  
  - O que não funcionou como o esperado?  
  - O que aprendeu sobre conversar com IAs?

