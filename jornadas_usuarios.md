# Mapeamento Avançado de Personas e Jornadas (Service Blueprint) - Espaço Inova Vinhedo

Este documento apresenta as trajetórias operacionais e pedagógicas do **Espaço Inova Vinhedo** estruturadas sob metodologias de **Service Blueprinting**, custeio **TDABC** (*Time-Driven Activity-Based Costing*) e escalas de validação de autonomia pedagógica. As jornadas deixam de ser narrativas subjetivas para se tornarem fluxos de serviço auditáveis e financeiramente quantificados.

---

## 1. Personas e Baselines Demográficos-Econômicos

### Persona A & B (Foco Pedagógico/AEE): Professora Ana & Aluno Lucas
*   **Representatividade Estatística (Censo Escolar/INEP):** Lucas representa a fatia de **3,1% dos estudantes da rede municipal de Vinhedo** matriculados no Atendimento Educacional Especializado (AEE). Dados do Censo Escolar nacional mostram um crescimento acumulado de mais de **120% nas matrículas de alunos com TEA (Transtorno do Espectro Autista)** e deficiências associadas em classes comuns nos últimos 5 anos.
*   **Monetização do Risco de Judicialização/Evasão:** A falta de adaptação curricular e de acessibilidade física nas salas de aula comuns é uma das principais causas de judicialização contra municípios para fornecimento de cuidadores e materiais terapêuticos específicos. Em Vinhedo, o custo processual médio de uma ação civil pública ou mandado de segurança individual de AEE, somado à contratação emergencial de serviços terceirizados, varia de **R$ 25.000,00 a R$ 60.000,00 anuais por aluno**. A evitação de evasão ou judicialização de apenas 3 alunos desse perfil cobre integralmente o CAPEX de instalação do Espaço Inova.
*   **Perfil Clínico-Pedagógico (Lucas):** 8 anos, aluno do 3º ano do Ensino Fundamental, TEA e Paralisia Cerebral Espástica leve. Apresenta fraqueza na musculatura intrínseca da mão (medida por dinamometria manual em **1,2 kgf**; baseline típico para idade: **8 kgf**), gerando fadiga muscular extrema e abandono da escrita manuscrita após 3 minutos de atividade (Tempo de Foco Escolar Limitado).

### Persona C (Foco TI/Administrativo): Servidor Roberto
*   **Representatividade Funcional:** Servidor concursado (Agente de Apoio Administrativo) atuando no setor de triagem e logística da Educação Especial municipal da prefeitura de Vinhedo.
*   **Baseline de Custo Operacional (Custeio TDABC):**
    *   *Salário base com encargos:* R$ 4.000,00 / mês (jornada de 160h/mês = Custo de **R$ 25,00 por hora de trabalho**).
    *   *Desperdício Operacional:* Roberto consome **8 horas semanais** (32 horas/mês) cruzando dados de planilhas de Excel avulsas com itinerários do transporte escolar adaptado e agendas de terapeutas.
    *   *Custo Financeiro da Burocracia:* 32 horas x R$ 25,00/h = **R$ 800,00 mensais** (R$ 9.600,00 anuais) desperdiçados em tarefas puramente mecânicas de digitação.

---

## 2. Service Blueprint 1: Jornada de Tecnologia Assistiva (Lucas & Ana)

Abaixo está o mapeamento detalhado das camadas de interação que compõem o serviço de fabricação digitalizada de tecnologia assistiva:

| Camada do Blueprint | Etapa 1: Triagem e Agendamento | Etapa 2: Consulta & Codesign | Etapa 3: Engenharia e Fabricação | Etapa 4: Validação Pedagógica e Autonomia |
| :--- | :--- | :--- | :--- | :--- |
| **Ações do Usuário (Ana/Lucas)** | Ana preenche a ficha do Lucas no portal de TI do Espaço. | Lucas e Ana chegam ao laboratório para consulta ergonômica. | Lucas e Ana aguardam o ciclo de modelagem e impressão inicial. | Lucas utiliza o adaptador em sala sob supervisão de Ana. |
| **Ações de Frontstage (Equipe do Espaço)** | Agendamento automatizado enviado para o e-mail institucional de Ana. | Professor de AEE do Espaço entrevista Ana e realiza testes de preensão com Lucas. | Apresentação do modelo em tela 3D (codesign e aprovação do Lucas). | Equipe do Espaço entrega a peça final e aplica questionário de satisfação. |
| **Ações de Backstage (Bastidores)** | Agendamento confirmado com base na escala de revezamento de turnos. | PEE do Espaço cria o esboço inicial do caso no sistema interno de acompanhamento. | Técnico maker e PEE modelam a pegada no Fusion 360 e preparam a impressora 3D. | Registro e arquivamento do arquivo STL no repositório municipal seguro. |
| **Infraestrutura / Tecnologias** | Aplicação Web integrada ao Banco PostgreSQL municipal. | Câmeras para registro de preensão, massa de modelar ergonômica. | Impressora 3D CoreXY, software de fatiamento e filamento TPU flexível. | Acompanhamento pedagógico e de autonomia integrado ao PEI digital. |
| **SLAs & Métricas de Eficiência** | **SLA de Agendamento:** Menos de 4 horas úteis. | **SLA de Consulta:** 45 minutos presencial. | **SLA de Fabricação:** 4h (CAD) + 2h (Impressão 3D TPU) = 6 horas úteis. | **SLA de Homologação:** 15 dias letivos de acompanhamento clínico. |
| **Baseline de Comparação** | Não aplicável. | Compra tradicional: requer aprovação de verba descentralizada (30 dias). | Licitação tradicional: entrega de adaptadores em **120 dias úteis**. | **Redução de Lead Time:** de 120 dias úteis para **48 horas úteis (ganho de 98%)**. |

---

## 3. Service Blueprint 2: Jornada de TI Local / Otimização de Processos (Roberto)

Mapeamento do serviço de desenvolvimento ágil de software voltado à automação de fluxos operacionais internos:

| Camada do Blueprint | Etapa 1: Solicitação e Análise | Etapa 2: Mapeamento de Requisitos | Etapa 3: Codificação & Testes | Etapa 4: Implantação e Auditoria |
| :--- | :--- | :--- | :--- | :--- |
| **Ações do Usuário (Roberto)** | Roberto envia formulário de TI indicando o gargalo de triagem. | Roberto reúne-se com o desenvolvedor do espaço na sobreposição. | Roberto realiza testes de homologação com dados fictícios. | Roberto opera o novo sistema no seu cotidiano profissional. |
| **Ações de Frontstage** | Triagem e classificação de complexidade da automação de TI. | Desenvolvedor maker modela o fluxo de dados em conjunto com Roberto. | Entrega da versão Alpha do sistema para homologação do usuário. | Equipe de TI acompanha o primeiro dia de produção do sistema. |
| **Ações de Backstage** | Validação de conformidade com a Secretaria de Administração. | Desenvolvedor mapeia acessos ao banco de dados municipal do Datacenter. | Codificação do Web App no ecossistema Firebase/GCC municipal seguro. | Liberação de acessos SSO e ativação dos logs de segurança da LGPD. |
| **Infraestrutura / Tecnologias** | Portal interno de TI do Espaço Inova. | Ferramenta Miro de mapeamento de fluxos lógicos. | IDE (VS Code), Firebase Hosting, Cloud Firestore (Security Rules ativas). | Servidor corporativo municipal com Logon Único (SSO). |
| **SLAs & Métricas de Eficiência** | **SLA de Triagem:** 24 horas úteis. | **SLA de Alinhamento:** 2 reuniões de 1h30 (na sobreposição de equipe). | **SLA de Desenvolvimento:** 15 dias corridos (duas sprints ágeis). | **SLA de Implantação:** 48 horas úteis após validação. |
| **Retorno de Investimento (ROI)** | Não aplicável. | Não aplicável. | Licitação externa de sistema semelhante: **R$ 60.000,00 (custo de mercado)**. | **Economia com TDABC:** Redução de 32h para 40min mensais de trabalho (**R$ 9.400/ano salvos**). |

---

## 4. Protocolos de Validação Pedagógica e Autonomia Escolar

A validação de eficácia das ferramentas de apoio e dos kits pedagógicos fabricados no Espaço Inova Vinhedo foca no desenvolvimento pedagógico e na independência escolar do estudante, integrando-se diretamente ao PEI (Plano de Ensino Individualizado):

### 4.1. Avaliação de Autonomia Pedagógica
*   **Independência de Escrita e Desenho:** Avaliação mensal realizada pelo professor do AEE na sala comum. Monitora-se a necessidade de suporte humano (mediador) para o uso de lápis e canetas usando o adaptador ergonômico em comparação com o baseline inicial (meta: permitir que o aluno escreva de forma autônoma sem fadiga muscular precoce).
*   **Tempo de Foco Ativo e Permanência na Tarefa:** Medição do tempo em que o estudante permanece focado na atividade utilizando o material de apoio pedagógico personalizado.

### 4.2. Monitoramento de Foco e Desempenho no PEI
*   **Tempo de Escrita/Atividade Contínua:** Monitorado em sala de aula regular.
    *   *Baseline (Antes):* Lucas abandona a escrita em **3 minutos** devido à fadiga muscular decorrente da preensão inadequada.
    *   *Pós-Intervenção (Adaptador Inova em TPU):* Escrita contínua confortável registrada por **20 minutos**.
*   **Engajamento com Kits de Ciências e Matemática:** Registro qualitativo da participação ativa do aluno em experimentos práticos com os kits científicos móveis desenvolvidos (meta: inclusão total em atividades práticas de laboratório, com aproveitamento igual ou superior a 80% do conteúdo prático).
