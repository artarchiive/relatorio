# Relatório de Design de Interação - Sprint 2
**Instituição:** Centro Universitário de Viçosa (UNIVIÇOSA)
**Curso:** Análise e Desenvolvimento de Sistemas (ADS 501)
**Professor:** Carlos Henrique Tavares Brumatti
**Empresa:** ByteCore Solutions
**Missao:** "Simplificar a interação entre cliente e empresa, eliminando barreiras de comunicação."
**Slogan:** *"Transformando ideias em tecnologia."*

---

## 1. Composição da Equipe e Papéis
* **Isaak** — CEO (Liderança estratégica e alinhamento de visão)
* **Elton** — Scrum Master (Facilitação ágil, gestão do Trello e controle de prazos/entregas)
* **Pedro Lacerda** — Product Owner (Visão de negócio, escopo e requisitos)
* **Equipe de Desenvolvimento & Design** (Execução técnica, UX/UI e implementação)

---

## 2. Descrição do Problema e da Solução

### 2.1 O Problema (Baseado em Pesquisa)
Identificamos que clientes locais de prestadores de serviços (salões de beleza, clínicas, consultórios) enfrentam barreiras críticas de tempo e comunicação. O agendamento tradicional via ligações telefônicas ou mensagens assíncronas no WhatsApp gera gargalos, longos tempos de espera e incerteza sobre a disponibilidade real de horários. 

Nossa persona mapeada, **Ana Martins** (32 anos, auxiliar administrativa), possui uma rotina severamente agitada entre trabalho e família. Ela apresenta altos níveis de ansiedade pela falta de confirmações imediatas e frequentemente desiste de agendar serviços quando o processo exige interações complexas ou demoradas.

### 2.2 A Solução Proposta
A **ByteCore Solutions** desenvolveu uma interface web responsiva com foco absoluto em usabilidade mobile-first. A plataforma elimina intermediários, permitindo que o usuário visualize a grade de horários disponíveis em tempo real e realize o agendamento completo em menos de um minuto. O sistema mitiga as dores da persona por meio de feedbacks visuais instantâneos de confirmação e um módulo integrado de simulação de lembretes automáticos, reduzindo o esquecimento e o no-show.

---

## 3. Especificação de Requisitos

### 3.1 Requisitos Funcionais (RF)
* **RF01 (Autenticação):** O sistema deve permitir que o usuário realize cadastro e login simples com e-mail e senha.
* **RF02 (Visualização em Tempo Real):** O sistema deve exibir uma grade interativa de horários livres filtrados por data e tipo de serviço, eliminando a incerteza de disponibilidade.
* **RF03 (Ação de Agendamento):** O sistema deve permitir que o cliente selecione o horário desejado e conclua a reserva em até 3 cliques a partir da tela inicial.
* **RF04 (Confirmação e Notificação):** O sistema deve exibir uma tela/modal de confirmação instantânea logo após a reserva e disparar uma simulação de lembrete automático.
* **RF05 (Gestão de Agenda):** O sistema deve disponibilizar um painel simplificado ("Meus Agendamentos") onde o usuário possa cancelar ou reagendar um compromisso sem burocracias.

### 3.2 Requisitos Não Funcionais (RNF)
* **RNF01 (Compatibilidade/Responsividade):** A interface deve ser totalmente responsiva e otimizada para smartphones (foco no Android, dispositivo principal da persona Ana Martins).
* **RNF02 (Usabilidade/UX):** A interface deve possuir baixa carga cognitiva, eliminando etapas desnecessárias para atender usuários com nível digital intermediário.
* **RNF03 (Segurança):** Os dados cadastrais e o histórico de agendamentos devem ser protegidos seguindo boas práticas de privacidade.
* **RNF04 (Disponibilidade):** A grade de agendamentos deve estar disponível para consultas 24 horas por dia, 7 dias por semana.

---

## 4. Protótipos e Decisões de Design (Figma)

*Conforme a diretriz obrigatória do projeto, todas as etapas de prototipação foram centralizadas na ferramenta Figma.*

### 4.1 Protótipo de Baixa Fidelidade (Wireframe)
* **Abordagem:** Estrutura baseada em blocos de conteúdo limpos, priorizando o fluxo vertical (Single Page Application - SPA) focado no ambiente mobile.
* **Decisões de Design:** Decidimos expor a grade de horários diretamente em botões do tipo "pills" (pastilhas) na tela inicial. Isso elimina a necessidade de menus suspensos escondidos, facilitando a interação de quem está acessando o app de forma rápida durante o intervalo de trabalho.

### 4.2 Protótipo de Alta Fidelidade e Identidade Visual
* **Tipografia:** Escolha de fontes Sans-serif limpas (como Inter ou Roboto), garantindo excelente legibilidade em telas de smartphones mesmo sob luz solar (dados móveis).
* **Paleta de Cores e Justificativas de Estilo:**
    * **Azul ardósia/Navy escuro (Principal):** Transmite a sobriedade, estabilidade e confiança técnica da marca *ByteCore Solutions*.
    * **Verde Esmeralda (Acentuação/Sucesso):** Utilizado estrategicamente nos estados de confirmação e sucesso. Essa cor atua diretamente no alívio da ansiedade da persona ao fornecer um feedback visual incontestável de que o agendamento foi fixado.
    * **Cinza Claro Neutro (Fundo):** Mantém o contraste alto sem agredir a visão, organizando as informações em cartões ("cards") flutuantes que delimitam as etapas do fluxo (Escolha do Serviço -> Data -> Horário).
