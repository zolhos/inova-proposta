# Cronograma Detalhado de Implementação - Espaço Inova Vinhedo

Este documento detalha o cronograma de implantação e operação do **Espaço Inova Vinhedo** ao longo de um horizonte de 8 meses, especificando para cada fase as atividades operacionais, os requisitos de entrada, as perguntas críticas de validação, os entregáveis tangíveis e os marcos de sucesso (*milestones*).

---

## 📅 Visão Geral do Cronograma

```
 Mês 1 ── Mês 2 ──────── Mês 3 ── Mês 4 ──────── Mês 5 ── Mês 6 ──────── Mês 7 ── Mês 8+
┌──────────────────────┬──────────────────────┬──────────────────────┬──────────────────┐
│ FASE 1: DIAGNÓSTICO  │ FASE 2: ESTRUTURAÇÃO │ FASE 3: PILOTO & CAP │ FASE 4: OPERAÇÃO │
│  Mapeamento & local  │  Reforma & Compras   │ Treinamento & Piloto │  Atendimentos    │
└──────────────────────┴──────────────────────┴──────────────────────┴──────────────────┘
```

---

## 🔍 Fase 1: Diagnóstico e Mapeamento (Mês 1 ao Mês 2)

### 1.1. Objetivo
Mapear as demandas reais de tecnologia assistiva nas salas de recursos multifuncionais de Vinhedo e selecionar o imóvel público que abrigará o laboratório.

### 1.2. Informações Necessárias para Execução (Inputs)
*   Censo de alunos matriculados no AEE de Vinhedo, subdividido por tipo de deficiência ou transtorno.
*   Inventário de imóveis públicos municipais disponíveis com acessibilidade física e facilidade de estacionamento.
*   Mapeamento das linhas de transporte escolar adaptado da prefeitura.

### 1.3. Perguntas Cruciais a Serem Respondidas
1.  *Quais são as 5 tecnologias assistivas ou materiais pedagógicos adaptados mais recorrentes e caros que as salas de AEE demandam hoje?*
2.  *O imóvel cogitado suporta a carga elétrica simultânea de computadores, impressoras 3D e o sistema de exaustão industrial da cortadora a laser (mínimo de 15kW de carga dedicada)?*
3.  *Como é a facilidade de acesso físico para cadeirantes na área de desembarque do local selecionado?*

### 1.4. Atividades Detalhadas
*   **A.1.1:** Realizar workshops com os professores de educação especial da rede municipal de Vinhedo para mapear gargalos didáticos.
*   **A.1.2:** Efetuar vistorias técnicas de engenharia elétrica e acessibilidade (NBR 9050) em até 3 locais pré-selecionados.
*   **A.1.3:** Redigir o termo de referência técnica para a compra das máquinas e insumos do laboratório.

### 1.5. Entregáveis e Marcos (Milestones)
*   📄 **Relatório de Mapeamento de Necessidades do AEE Vinhedo:** Documento contendo as principais demandas de TA e os perfis clínicos prioritários.
*   📄 **Laudo de Escolha e Adequação do Imóvel:** Estudo técnico de engenharia justificando a seleção do local físico e descrevendo as reformas elétricas necessárias.
*   🚩 **Milestone 1:** Imóvel definido e Termo de Referência homologado para licitação.

---

## 🔨 Fase 2: Estruturação e Infraestrutura (Mês 2 ao Mês 4)

### 2.1. Objetivo
Reforma física do espaço físico e aquisição/instalação de toda a infraestrutura de fabricação digital, computadores e mobiliário.

### 2.2. Informações Necessárias para Execução (Inputs)
*   Projetos executivos de elétrica, iluminação e exaustão industrial de ar do laboratório.
*   Ata de Registro de Preços ou editais de pregão vigentes na prefeitura de Vinhedo para equipamentos de TI e móveis.
*   Especificações de segurança da cortadora a laser (comprimento de onda, gases gerados, enclausuramento).

### 2.3. Perguntas Cruciais a Serem Respondidas
1.  *A tubulação de exaustão da cortadora a laser possui filtros de carvão ativo adequados para eliminar os odores de corte de acrílico e MDF, evitando reclamações da vizinhança ou poluição ambiental?*
2.  *Os computadores licitados possuem placas de vídeo dedicada básicas homologadas para rodar programas de modelagem CAD sem lentidão?*
3.  *O layout físico garante a separação estrita da "zona de sujeira" (laser e marcenaria manual) e da "zona limpa" (computadores, eletrônica e atendimento clínico de AEE)?*

### 2.4. Atividades Detalhadas
*   **A.2.1:** Executar a reforma física (pintura, piso tátil, bancadas reforçadas, instalação elétrica e de exaustor).
*   **A.2.2:** Realizar o processo de compra e recebimento técnico das impressoras 3D, cortadora a laser e computadores de design.
*   **A.2.3:** Instalação e teste de calibração preliminar do maquinário.
*   **A.2.4:** Configuração da rede segura de TI da prefeitura (SSO e logs) e instalação de softwares open-source.

### 2.5. Entregáveis e Marcos (Milestones)
*   👷 **Espaço Físico Reformado e Homologado:** Local com instalações elétricas e exaustão instaladas e atestadas por laudo de segurança.
*   📦 **Inventário Físico de Equipamentos Instalados:** Relatório técnico de calibração e teste de funcionamento inicial de 100% do maquinário do FabLab.
*   🚩 **Milestone 2:** Equipamentos instalados, calibrados e rede municipal de TI ativa no local.

---

## 🎓 Fase 3: Capacitação da Equipe e Projeto Piloto (Mês 5 ao Mês 6)

### 3.1. Objetivo
Treinar e certificar a equipe de 4 servidores públicos municipais e executar o projeto piloto de fabricação de tecnologia assistiva e o primeiro aplicativo web.

### 3.2. Informações Necessárias para Execução (Inputs)
*   Designações oficiais de RH dos 4 servidores que comporão a equipe de revezamento.
*   Manuais e tutoriais rápidos de operação segura e preventiva das impressoras e laser.
*   Fichas de 10 alunos do AEE selecionados para o projeto piloto.

### 3.3. Perguntas Cruciais a Serem Respondidas
1.  *Os servidores designados atingiram a proficiência básica operacional necessária para operar a cortadora a laser de forma autônoma e segura?*
2.  *Os protótipos em TPU flexível e MDF criados no piloto foram bem recebidos e validados pelos terapeutas e professores de AEE nas escolas piloto?*
3.  *O fluxo de sobreposição diária da equipe (12:30 às 17:00) está funcionando com sinergia produtiva?*

### 3.4. Atividades Detalhadas
*   **A.3.1:** Executar a trilha de capacitação prática dos servidores (40 horas de treinamento em modelagem 3D, corte laser, Arduino e governança LGPD).
*   **A.3.2:** Desenvolver e testar o codesign de 10 dispositivos assistivos personalizados (piloto).
*   **A.3.3:** Desenvolver e homologar o primeiro aplicativo local de TI municipal (painel de agendamento do AEE).
*   **A.3.4:** Colher assinaturas dos Termos de Consentimento (TCLE) dos responsáveis dos alunos do piloto.

### 3.5. Entregáveis e Marcos (Milestones)
*   📜 **Certificados de Capacitação Técnica Maker:** Comprovação da formação operacional dos servidores designados.
*   ♿ **Lote Piloto de Tecnologias Assistivas Homologadas:** Entrega de 10 dispositivos nas escolas parceiras com relatórios clínicos de evolução inicial (QUEST/AHA).
*   💻 **Web App de Agendamento do AEE (Versão 1.0):** Aplicativo implantado em ambiente seguro de produção do município.
*   🚩 **Milestone 3:** Piloto concluído e homologado em ambiente escolar; equipe capacitada.

---

## 🚀 Fase 4: Operação Plena e Expansão (Mês 7 em diante)

### 4.1. Objetivo
Estabelecer o atendimento público regular aos alunos do AEE, professores e secretarias municipais, escalando a fabricação digital e o desenvolvimento ágil.

### 4.2. Informações Necessárias para Execução (Inputs)
*   Calendário letivo anual da rede municipal de Vinhedo.
*   Registro e triagem automatizada de demandas inseridas no portal de TI pelo web app.
*   Contratos de fornecimento ou Notas de Doação de MDF/acrílico (Logística Reversa).

### 4.3. Perguntas Cruciais a Serem Respondidas
1.  *O laboratório está operando dentro das metas estabelecidas de lead time (entrega de recursos de AEE em menos de 15 dias úteis)?*
2.  *Os indicadores qualitativos de longo prazo (evolução no PEI, redução de evasão de alunos PCD/TEA) mostram tendência de melhora consistente?*
3.  *Quantas empresas locais do distrito industrial de Vinhedo estão engajadas ativamente na logística reversa e usando o selo "Empresa Parceira da Inclusão"?*

### 4.4. Atividades Detalhadas
*   **A.4.1:** Executar a escala de revezamento contínuo das equipes para atendimento ao público das 08:30 às 20:30.
*   **A.4.2:** Fabricar sob demanda os dispositivos pedagógicos solicitados e homologados pelas salas de AEE.
*   **A.4.3:** Realizar as visitas de planejamento pedagógico (HTPC Maker) com as escolas municipais.
*   **A.4.4:** Consolidar mensalmente o painel de KPIs (economicidade e desenvolvimento no PEI) para envio ao Prefeito e Controle Interno.

### 4.5. Entregáveis e Marcos (Milestones)
*   📂 **Portfólio de Dispositivos e Modelos Digitais Municipais:** Repositório Git público atualizado contendo os arquivos STL e códigos-fonte anonimizados criados em Vinhedo.
*   📊 **Relatório Semestral de Impacto e Economicidade Pública:** Documento de prestação de contas demonstrando a economia líquida gerada e o payback do laboratório.
*   🚩 **Milestone 4:** Operação estável e primeiro ciclo semestral de economia atestado pela Controladoria Geral do Município.
