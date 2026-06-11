# Relatório de Aprimoramento Técnico e Político-Regulatório
## Projeto: Espaço Inova Vinhedo (Laboratório Maker Municipal)

Este relatório, elaborado sob a ótica de um **Especialista Sênior em Projetos e Políticas Públicas**, apresenta a análise crítica, a exploração estratégica e o aprimoramento substancial da proposta do **Espaço Inova Vinhedo**. O objetivo é elevar o nível de maturidade técnica, regulatória e financeira do projeto para viabilizar sua aprovação por órgãos de controle e sua elegibilidade a editais públicos de fomento (como FINEP, FAPESP e BNDES), garantindo uma implementação exequível em um prazo máximo de 12 meses.

---

## 1. 🌲 Exploração de Ideias (Tree of Thoughts)

Para alinhar o Espaço Inova Vinhedo com as diretrizes e metas de políticas públicas federais e estaduais, foram desenvolvidas três perspectivas estratégicas complementares:

### Perspectiva 1: Inclusão Escolar Multissensorial e Universal (Alinhamento com a LBI e PNEE)
*   **Foco:** O laboratório como um acelerador de acessibilidade escolar no âmbito do Atendimento Educacional Especializado (AEE).
*   **Fundamento:** Embasado na Lei Brasileira de Inclusão da Pessoa com Deficiência (LBI - Lei nº 13.146/2015) e no Plano Nacional de Educação Especial (PNEE). A manufatura aditiva (impressão 3D) e o corte a laser deixam de ser "atividades recreativas" e passam a ser ferramentas de fornecimento de adaptadores escolares ergonômicos e materiais didáticos de Design Universal para a Aprendizagem (DUA).
*   **Mecanismo:** Integração direta dos recursos produzidos ao Plano de Ensino Individualizado (PEI) de cada aluno com deficiência, Transtorno do Espectro Autista (TEA) ou altas habilidades, reduzindo o tempo de espera das aquisições de 12 meses (via licitação convencional) para 15 dias úteis.

### Perspectiva 2: Descentralização do Ensino Científico Prático (Kits de Ciências e Matemática)
*   **Foco:** Melhoria do IDEB, democratização do STEM (*Science, Technology, Engineering, and Math*) e infraestrutura escolar.
*   **Fundamento:** Embasado nas metas de educação científica da Base Nacional Comum Curricular (BNCC). O laboratório maker atua como uma fábrica pública centralizada que produz e distribui kits de experimentos científicos e pedagógicos móveis para suprir as escolas municipais de Vinhedo que não dispõem de laboratório físico de ciências.
*   **Mecanismo:** Fabricação sob demanda de kits de física (roldanas, polias, ótica), biologia (modelos celulares tridimensionais), química (tabelas e moldes) e matemática (réguas e frações táteis) em MDF e filamento plástico a frações do custo do mercado privado de suprimentos escolares.

### Perspectiva 3: GovTech, Modernização Administrativa e Eficiência Fiscal
*   **Foco:** Descentralização da inovação no setor público e autonomia digital do município.
*   **Fundamento:** Alinhamento com a Lei do Governo Digital (Lei nº 14.129/2021) e o Marco Legal das Startups (Lei Complementar nº 182/2021). O laboratório atua como uma incubadora GovTech interna, utilizando recursos próprios de tecnologia da informação para o desenvolvimento ágil de soluções públicas de baixo custo.
*   **Mecanismo:** Substituição de contratos comerciais fechados de software por plataformas web municipais leves desenvolvidas em servidores locais de nuvem (como instâncias institucionais de Firebase/Google Cloud), reduzindo custos de licenças e promovendo a inovação aberta.

---

## 2. 🔍 Análise Passo a Passo (Mapeamento de Lacunas)

A avaliação minuciosa da documentação original revelou 5 lacunas críticas que poderiam causar a rejeição do projeto em auditorias do Tribunal de Contas do Estado (TCE-SP) ou a desqualificação em editais de fomento:

### ⚠️ Lacuna 1: Complexidade Regulatória Sanitária Imediata (ANVISA RDC nº 925/2024)
O projeto original prevê a fabricação de órteses personalizadas de posicionamento de punho em PETG e adaptadores clínicos. No Brasil, órteses e próteses são classificadas pela ANVISA como **Dispositivos Médicos Personalizados sob Medida**. A fabricação imediata desses itens no laboratório maker sem uma estrutura de convênio de saúde, e sem a contratação/supervisão de um Responsável Técnico (RT) devidamente credenciado (Terapeuta Ocupacional ou Fisioterapeuta) registrado no CREFITO-3, exporia a prefeitura a severos riscos de responsabilidade civil e criminal por exercício ilegal da medicina/saúde pública. A solução é uma **abordagem bifásica**, focando a Fase 1 (12 meses) em objetos pedagógicos auxiliares de baixo risco que são isentos de regulação pela ANVISA por não possuírem finalidade terapêutica clínica direta.

### ⚠️ Lacuna 2: Inconsistência de Custos e BDI no CAPEX e OPEX
A planilha orçamentária do projeto original está baseada em preços comuns do varejo eletrônico (ex: impressoras 3D Bambu Lab P1S por R$ 8.500,00). Na administração pública (Lei nº 14.133/2021), as aquisições por pregão envolvem custos adicionais de frete homologado, garantias estendidas (*on-site* por 12 a 36 meses), suporte pós-venda, conformidades fiscais e BDI (Benefício e Despesas Indiretas) dos licitantes, o que costuma inflacionar os preços reais em 20% a 30%. Equipamentos críticos de segurança (EPIs, lava-olhos, exaustão de segurança) e custos de descarte de resíduos químicos foram omitidos.

### ⚠️ Lacuna 3: Fragilidade Arquitetural e de Segurança da Equipe GovTech (LGPD)
O modelo de "TI Local" atribui a um único "Técnico de TI" (com jornada dividida com manutenção de hardware) a responsabilidade por projetar, codificar, implantar e manter múltiplos softwares públicos. Essa estrutura gera um ponto crítico de falha (*bus factor* igual a 1). Adicionalmente, sistemas do AEE lidam com dados altamente sensíveis de menores e laudos clínicos. A ausência de uma arquitetura segura de dados, regras claras de criptografia em trânsito e em repouso, políticas de controle de acesso de usuários e um protocolo estrito de conformidade com a LGPD (Lei Geral de Proteção de Dados Pessoais - Lei nº 13.709/2018) inviabiliza juridicamente o uso dessas plataformas pela prefeitura.

### ⚠️ Lacuna 4: Falta de Licenciamento Ambiental e Gestão de Resíduos (PNRS)
A operação de impressoras de resina (MSLA) gera resíduos químicos perigosos (isopropanol saturado de fotopolímero tóxico não curado e recipientes de resina vazios). A cortadora a laser CO2 emite gases de queima de acrílico e MDF (ricos em formaldeídos). A ausência de um sistema certificado de exaustão com filtragem de carvão ativo e HEPA, aliada à falta de um contrato de coleta e destinação final de resíduos industriais perigosos (Classe I), fere a Política Nacional de Resíduos Sólidos (PNRS) e pode acarretar interdição por órgãos ambientais (CETESB).

### ⚠️ Lacuna 5: Segregação Física Insuficiente e Riscos de Contaminação
O corte de MDF e marcenaria de bancada geram micropartículas de serragem suspensas no ar. A poeira de madeira destrói os rolamentos das impressoras 3D FDM, contamina as cubas de resina líquida das impressoras MSLA e queima placas eletrônicas e lentes ópticas da cortadora a laser. O layout orçado de 120m² não pode ser apenas "dividido em áreas conceituais", sob risco de inutilizar o maquinário em poucos meses. É obrigatória uma segregação física estrutural por meio de divisórias adequadas e zonas com diferença de pressão ou purificação ativa de ar.

---

## 3. 💡 Recomendações de Melhoria

Para suprir as lacunas acima, as seguintes melhorias estruturais devem ser aplicadas ao projeto:

1.  **Divisão do Escopo em Abordagem Bifásica (Fase 1 - Exequível):**
    *   **Fase 1 (Meses 1 a 12):** Foco 100% pedagógico. Fabricação de kits didáticos de ciências e matemática para as escolas e de adaptadores auxiliares de escrita e rotina escolar de baixo risco (engrossadores, acionadores, guias de leitura). Esses itens são classificados como insumos pedagógicos escolares e, por não possuírem indicação ou alegação terapêutica direta, são **isentos de regulação e licenciamento pela ANVISA**.
    *   **Fase 2 (A partir do Mês 13 - Expansão):** Ampliação para Tecnologia Assistiva sob medida (órteses de punho) após estruturação de convênio técnico com a Secretaria de Saúde do município e designação de um Responsável Técnico (TO ou Fisioterapeuta) habilitado no CREFITO-3.
2.  **Adequação do Orçamento Público (CAPEX/OPEX):** Reajustar as planilhas aplicando uma margem de segurança de licitação de 20% a 30%, além de discriminar sistemas industriais de exaustão forçada, EPIs específicos, câmara lava-olhos e contrato de coleta de resíduos químicos industriais (vinculado à limpeza de impressoras de resina).
3.  **Segregação Física das Zonas de Trabalho:** Detalhar a planta do laboratório prevendo isolamento físico entre a **Zona de Poeira (Marcenaria/Laser)** e a **Zona Limpa de Alta Precisão (Impressão 3D/Eletrônica/TI)** com portas herméticas e purificação de ar ativa na Zona Limpa.
4.  **Pipeline de Desenvolvimento Seguro e LGPD para GovTech:** Estabelecer uma arquitetura de software utilizando a infraestrutura de TI central do município com criptografia ponta a ponta (HTTPS/TLS 1.3), bancos de dados segregados e anonimizados, autenticação integrada ao sistema da prefeitura e supervisão do Encarregado de Proteção de Dados (DPO) do município.
5.  **Minuta de Decreto de Resíduos para Economia Circular:** Formalizar as bases tributárias e operacionais da logística reversa, com apoio do Regulamento do ICMS (RICMS-SP) e minutas de doação industrial sem incidência tributária.

---

## 4. 📝 Seções Aprimoradas do Projeto (Prontas para Edital)

Abaixo estão reescritas as seções críticas do projeto original, adotando redação técnica de excelência, fundamentação legislativa nacional e rigor administrativo.

### 4.1. Abordagem Bifásica e Conformidade Sanitária (ANVISA)

O desenvolvimento de soluções de acessibilidade física e cognitiva no Espaço Inova Vinhedo dar-se-á por meio de uma abordagem incremental dividida em duas fases distintas:

```
┌────────────────────────────────────────────────────────────────────────┐
│              FASE 1 (Meses 1 a 12): ESCOPO PEDAGÓGICO                  │
├────────────────────────────────────────────────────────────────────────┤
│ - Desenvolvimento de adaptadores escolares ergonômicos (TPU flexível). │
│ - Fabricação de Kits Didáticos de Ciências e Matemática (MDF / FDM).   │
│ - Isenção ANVISA: Peças sem indicação terapêutica direta.              │
└──────────────────────────────────┬─────────────────────────────────────┘
                                   │
                                   ▼ (Marcos de Transição)
                       - Convênio Técnico SME + SMS
                       - Designação de TO/Fisioterapeuta RT
                                   │
                                   ▼
┌────────────────────────────────────────────────────────────────────────┐
│             FASE 2 (Meses 13+): TECNOLOGIA ASSISTIVA CLÍNICA           │
├────────────────────────────────────────────────────────────────────────┤
│ - Fabricação de órteses personalizadas sob medida (RDC 925/2024).      │
│ - Controle de biocompatibilidade de polímeros (ISO 10993).             │
│ - Acompanhamento clínico e supervisão do Responsável Técnico.          │
└────────────────────────────────────────────────────────────────────────┘
```

1.  **Fase 1 - Insumos Escolares Auxiliares (Isenção ANVISA):** Durante os primeiros 12 meses de funcionamento do laboratório maker, as atividades estarão focadas exclusivamente em materiais didáticos e recursos auxiliares escolares de uso cotidiano (tais como engrossadores de lápis, guias táteis de dislexia, acionadores simples de computador, tabuleiros de comunicação pedagógica e maquetes de relevo). Conforme as normas da ANVISA, por se tratarem de ferramentas de apoio ao aprendizado escolar regular e não possuírem finalidade ou alegação de reabilitação clínico-terapêutica, estes objetos **não são classificados como dispositivos médicos**, estando isentos de registros sanitários e de responsabilidade técnica em saúde.
2.  **Fase 2 - Tecnologia Assistiva sob Medida (RDC ANVISA nº 925/2024):** A expansão das atividades do laboratório para a confecção de órteses e próteses sob medida (dispositivos de saúde) dar-se-á de forma programada a partir do Mês 13, mediante a formalização de um **Convênio de Cooperação Técnica Intersecretarial** entre as Secretarias de Educação e de Saúde. Esta fase exigirá a designação de um **Responsável Técnico (RT)** habilitado da rede de saúde (Terapeuta Ocupacional ou Fisioterapeuta) para prescrever, modelar e assinar os termos de conformidade e uso de cada dispositivo clínico, garantindo rastreabilidade e controle absoluto em consonância com a legislação sanitária federal.

---

### 4.2. Diretrizes do Espaço Físico, Segurança Ocupacional e Gestão de Resíduos (PNRS)

O espaço físico será estruturado em duas salas isoladas para garantir a durabilidade dos aparelhos eletrônicos e a segurança dos usuários:

```
  =========================================
  ||             PLANTA FISICA            ||
  =========================================
  ||  ZONA DE POEIRA E CORTE               ||
  ||  - Cortadora Laser CO2 (Exaustão)     ||
  ||  - CNC / Marcenaria Leve              ||
  ||  - Coleta de Resíduos de MDF          ||
  ==================== PORTA DUPLA ========
  ||  ZONA LIMPA DE ALTA PRECISÃO          ||
  ||  - Impressoras 3D FDM e SLA           ||
  ||  - Bancada de Eletrônica e Solda      ||
  ||  - Estações de Programação e Computadores
  ||  - Climatização e Pressão Positiva    ||
  =========================================
```

1.  **Segregação Estrutural das Zonas:**
    *   **Zona A (Poeira e Alta Temperatura):** Abriga a cortadora a laser, furadeiras, lixadeiras e serras. Possui piso antiderrapante e divisórias de painéis termoacústicos com atenuação de 35dB.
    *   **Zona B (Zona Limpa e TI):** Abriga as impressoras 3D FDM/MSLA, bancadas de eletrônica com revestimento antiestático (ESD) e computadores de modelagem. Esta sala operará com sistema de ar condicionado com filtros purificadores e pressão ligeiramente positiva para impedir a entrada de partículas suspensas vindas da Zona A.
2.  **Sistema de Exaustão de Gases:** A cortadora a laser CO2 será conectada a um exaustor centrífugo industrial de 1.5 HP, operando com vazão mínima de $800\text{ m}^3/\text{h}$, com tubulação estanque de alumínio direcionada para chaminé externa elevada (mínimo de 3 metros acima do telhado). O sistema integrará um **filtro purificador ativo composto por barreira HEPA (particulados) e leito de carvão ativado (gases nocivos)**, atendendo às exigências da CETESB para emissões atmosféricas.
3.  **Segurança e EPIs:**
    *   Instalação obrigatória de 1 **Estação Lava-Olhos** de emergência integrada à rede hidráulica na Zona Limpa.
    *   Instalação de sensores eletrônicos de fumaça, monóxido de carbono e chamas interligados a disjuntores gerais.
    *   Uso mandatório de óculos de proteção com densidade óptica (OD) específica para o comprimento de onda do laser de CO2 ($10.600\text{ nm}$).
    *   Uso de máscaras semi-faciais com filtros para vapores orgânicos e gases ácidos durante a manipulação e limpeza química de resinas fotopolimerizáveis.
4.  **Gestão de Resíduos Químicos (PNRS - Lei nº 12.305/2010):**
    *   O laboratório possuirá 1 armário corta-fogo metálico para estocagem de solventes e reagentes (álcool isopropílico e resinas).
    *   Toda a lavagem de peças de resina será feita em recipientes estanques fechados. O álcool saturado com polímeros e as embalagens de resina usadas serão armazenados em tambores homologados de polietileno de alta densidade (PEAD).
    *   O município manterá contrato ativo com empresa especializada de engenharia ambiental para a coleta semestral, transporte e incineração segura (co-processamento) dos resíduos químicos perigosos (Código de Resíduo Classe I).

---

### 4.3. Arquitetura de TI, Segurança Cibernética e LGPD (Lei nº 13.709/2018)

As soluções digitais desenvolvidas na modalidade "TI Local" pelo Espaço Inova serão implantadas segundo rigorosas diretrizes de engenharia de software e privacidade de dados:

1.  **Governança de Dados de Menores:** Conforme o Artigo 14 da LGPD, o tratamento de dados pessoais de crianças e adolescentes exige consentimento específico dado por pelo menos um dos pais ou responsável legal.
    *   O laboratório utilizará o **Termo de Consentimento Livre e Esclarecido (TCLE) Digital**, integrado à autenticação do responsável via plataforma gov.br.
    *   Laudos e informações pedagógicas de AEE (dados pessoais sensíveis, conforme Artigo 5º, II da LGPD) serão **criptografados no banco de dados em repouso (AES-256)** e associados a chaves estrangeiras com identificadores UUIDv4. Nomes reais dos alunos e suas condições não serão gravados em tabelas comuns de rastreio de atividades das secretarias.
2.  **Infraestrutura e Hospedagem Segura:**
    *   Os aplicativos municipais serão hospedados no Datacenter Central da Prefeitura de Vinhedo ou na nuvem governamental contratada, utilizando a organização oficial de nuvem do município (com gestão de acesso IAM).
    *   O fluxo de tráfego de rede exigirá tráfego seguro obrigatório por meio do protocolo **HTTPS com TLS 1.3** e certificados SSL atualizados.
3.  **Pipeline de DevOps e Segurança de Código:**
    *   Os códigos-fonte dos softwares municipais serão hospedados em repositório Git corporativo fechado da prefeitura.
    *   Antes de cada publicação em ambiente de produção, o código será submetido a testes automatizados de segurança estática (SAST - *Static Application Security Testing*) para mitigar vulnerabilidades comuns do OWASP Top 10 (como injeção de SQL e XSS).
    *   O Encarregado de Proteção de Dados (DPO) da prefeitura realizará auditorias anuais de conformidade nas bases de dados dos sistemas desenvolvidos pelo laboratório.

---

### 4.4. Modelo Orçamentário Adequado a Editais de Licitação e Fomento (FINEP/BNDES)

O orçamento a seguir foi reajustado para incluir margens de licitação da Lei nº 14.133/2021, custos de frete homologado, garantias contratuais de 12 meses, sistemas de proteção ambiental e gestão de resíduos químicos.

#### 4.4.1. Investimento Inicial (CAPEX Ajustado)

| Item | Descrição Técnica e Requisitos de Licitante | Qtd | Valor Unit. Médio (c/ BDI/Tributos) | Valor Total Reajustado |
| :--- | :--- | :---: | :---: | :---: |
| **Cortadora a Laser CO2 (80W)** | Área de corte de 90x60cm, potência de 80W reais, Chiller industrial CW-5200, compressor integrado e lente de foco reserva. Garantia de 12 meses *on-site*. | 1 | R$ 42.000,00 | R$ 42.000,00 |
| **Impressora FDM CoreXY Fechada** | Câmara termicamente controlada, velocidade mínima de $350\text{ mm/s}$, bicos endurecidos de troca rápida, sensor de fim de filamento, câmera de monitoramento. Ex: Bambu Lab P1S ou similar corporativa. | 2 | R$ 10.500,00 | R$ 21.000,00 |
| **Impressora 3D de Resina MSLA** | Tela mono LCD com resolução mínima de 8K (ex: Elegoo Saturn 3 Ultra ou similar), cuba de resina metálica e exaustor de carvão ativo integrado. | 1 | R$ 6.500,00 | R$ 6.500,00 |
| **Estação de Cura e Lavagem UV** | Unidade de lavagem com hélice magnética e câmara de cura ultravioleta integrada com rotação automatizada ($360^\circ$). | 1 | R$ 3.000,00 | R$ 3.000,00 |
| **Plotter de Recorte de Vinil** | Boca de corte mínima de 60cm, sensor de leitura óptica de contorno, pedestal de suporte integrado e software licenciado de edição. | 1 | R$ 4.500,00 | R$ 4.500,00 |
| **Bancadas de Eletrônica ESD e Solda**| Estações de solda de alta precisão com controle digital de temperatura e extrator de fumaça de bancada com barreira de carvão ativo. | 2 | R$ 2.500,00 | R$ 5.000,00 |
| **Kits Educacionais de Robótica** | Microcontroladores (Arduino Uno R4, ESP32-S3 e Raspberry Pi Pico H), módulos de sensores de presença, motores de passo e servos. | 15 | R$ 400,00 | R$ 6.000,00 |
| **Ferramentas Manuais e EPIs** | Retíficas de alta precisão, parafusadeiras industriais, serras de bancada, óculos laser $10.600\text{ nm}$ e máscaras de gases respiratórias. | 1 | R$ 7.500,00 | R$ 7.500,00 |
| **Computadores de Modelagem/CAD** | Workstations corporativas i7, 32GB RAM DDR5, SSD NVMe 1TB, GPU dedicada NVIDIA RTX 4060 ou superior, monitor IPS 24" e Windows 11 Pro. | 4 | R$ 9.200,00 | R$ 36.800,00 |
| **Notebook para Coordenação** | Portátil corporativo i5, 16GB RAM, SSD 512GB, tela de 14", alta autonomia de bateria. | 1 | R$ 6.000,00 | R$ 6.000,00 |
| **Mobiliário Técnico Estrutural** | Bancadas mecânicas de madeira maciça, armário corta-fogo para químicos, mesas de informática integradas e divisórias acústicas. | 1 | R$ 22.000,00 | R$ 22.000,00 |
| **Infraestrutura Elétrica Dedicada** | Quadro elétrico exclusivo, cabos blindados de 6mm², sistema de aterramento TT exclusivo com DPS e interruptores DR independentes. | 1 | R$ 15.000,00 | R$ 15.000,00 |
| **Climatização e Purificação de Ar** | Ar condicionado split de 24.000 BTUs com ciclo reverso e purificador portátil com filtro HEPA de grau hospitalar. | 1 | R$ 10.000,00 | R$ 10.000,00 |
| **Segurança e Proteção contra Incêndio** | Estação Lava-Olhos de parede, 2 extintores de CO2 de 6kg, 2 extintores PQS de 6kg e sensores eletrônicos de gás de monóxido de carbono. | 1 | R$ 5.500,00 | R$ 5.500,00 |
| **CAPEX TOTAL AJUSTADO** | | | | **R$ 188.800,00** |

#### 4.4.2. Custeio Anual Recorrente (OPEX Ajustado)

| Categoria | Descrição do Insumo e Custeio Operacional | Consumo Mensal | Custo Anual Est. |
| :--- | :--- | :---: | :---: |
| **Filamentos 3D Certificados** | Filamento PLA, TPU Flexível e PETG de fabricante nacional homologado com certificação de atoxidade para uso escolar (12 kg/mês). | R$ 1.500,00 | R$ 18.000,00 |
| **Resina MSLA e Consumíveis SLA** | Resina acrílica padrão, resina do tipo dura/engenharia e resina flexível para produção de adaptadores escolares (1,5 L/mês). | R$ 800,00 | R$ 9.600,00 |
| **Insumos de Corte (MDF e Acrílico)**| Chapas virgens de MDF (3 e 6mm) e acrílico cast ($90\times60\text{cm}$) para kits didáticos complementares à logística reversa. | R$ 2.000,00 | R$ 24.000,00 |
| **Químicos e Solventes de Limpeza** | Álcool Isopropílico 99.8% de pureza e recipientes de lavagem especiais (30 L/mês). | R$ 300,00 | R$ 3.600,00 |
| **Componentes e Reposição Eletrônica** | Conectores, fios AWG, transistores, placas de fenolite cobreadas virgens para corrosão e reposição de kits de robótica desgastados. | R$ 666,66 | R$ 8.000,00 |
| **Manutenção Corretiva e Calibração** | Contrato de calibração anual dos computadores de modelagem e reposição de bicos endurecidos, correias e lubrificantes especiais. | - | R$ 12.000,00 |
| **Descarte e Coleta de Químicos** | Contrato de coleta e destinação final de resíduos Classe I com empresa licenciada junto à CETESB e IBAMA. | - | R$ 6.000,00 |
| **Energia Elétrica e Conectividade** | Rateio incremental de consumo elétrico industrial da cortadora laser e link dedicado de fibra óptica municipal de $200\text{ Mbps}$. | R$ 1.000,00 | R$ 12.000,00 |
| **Treinamento e Recertificação** | Custeio anual de cursos de capacitação técnica avançada em manufatura aditiva, modelagem e robótica para a equipe de servidores. | - | R$ 8.000,00 |
| **Licenças e Assinaturas Digitais** | Foco em pacotes livres e open source (Slic3r, FreeCAD, KiCAD). Licença do SO Windows Pro integrada ao CAPEX das máquinas. | R$ 0,00 | R$ 0,00 |
| **OPEX TOTAL ANUAL AJUSTADO** | | **R$ 6.266,66** | **R$ 101.200,00** |

---

### 4.5. Recursos Humanos, Papéis e Matriz de Governança Intersecretarial

A operação contínua do Espaço Inova Vinhedo na Fase 1 apoia-se em equipe baseada exclusivamente em servidores municipais da Secretaria de Educação e Administração, reduzindo a complexidade de contratações externas:

#### 4.5.1. Quadro de Pessoal e Atribuições Clínico-Técnicas (Fase 1)

```
                  ┌────────────────────────────────────────┐
                  │          COMITÊ GESTOR INOVA           │
                  │   (Educação, Administração, Des. Eco.) │
                  └───────────────────┬────────────────────┘
                                      │
                                      ▼
                  ┌────────────────────────────────────────┐
                  │   COORDENADOR PEDAGÓGICO DE INOVAÇÃO   │
                  │        (Gestão Geral do Laboratório)   │
                  └──────┬──────────────────────────┬──────┘
                         │                          │
                         ▼                          ▼
            ┌─────────────────────────┐ ┌─────────────────────────┐
            │   EQUIPE MULTIDISCIPLINAR│ │   DESENVOLVIMENTO DE TI │
            │      E TECNOLOGIA       │ │    E SUPORTE TÉCNICO    │
            │  - Professores de AEE   │ │  - Técnico de TI        │
            │    (Inclusão & Codesign)│ │  - Analista de Sistemas │
            └─────────────────────────┘ └─────────────────────────┘
```

1.  **Coordenador Pedagógico de Inovação (1 PEB II - 40h semanais):**
    *   *Papel Jurídico:* Gestor Administrativo do Espaço Maker.
    *   *Atribuições:* Coordenar a agenda de projetos e os atendimentos de AEE; responder perante o comitê intersecretarial municipal; autorizar o regime de pronto pagamento para compras emergenciais de insumos; liderar as campanhas de engajamento pedagógico nas escolas municipais de Vinhedo.
2.  **Professores de Educação Especial - Especialistas em AEE (2 PEE - 30h/40h semanais):**
    *   *Papel Pedagógico:* Especialistas em Codesign Inclusivo de Apoio Escolar.
    *   *Atribuições:* Mapear barreiras cognitivas e físicas de aprendizagem nas salas de recursos multifuncionais; entrevistar estudantes e seus responsáveis; conduzir oficinas temáticas integradas de robótica sensorial, cartografia multissensorial e montagem de kits didáticos de ciências; validar a aplicabilidade prática dos recursos pedagógicos produzidos em sala de aula comum.
3.  **Técnico de Suporte e Desenvolvimento Local (1 Servidor TI - 40h semanais):**
    *   *Papel Tecnológico:* Administrador de Máquinas e Desenvolvedor de Software.
    *   *Atribuições:* Executar a manutenção preventiva, nivelamento de mesa e calibração fina das impressoras 3D; calibrar lentes e exaustor da cortadora a laser; codificar, auditar e testar os sistemas municipais do pipeline GovTech, garantindo a integridade dos dados e o cumprimento da LGPD sob orientação do DPO municipal.
4.  **Profissionais de Saúde (Terapeuta Ocupacional/Fisioterapeuta) - Fase 2:**
    *   Estes profissionais serão integrados às atividades do laboratório de forma pontual e parcial a partir do Mês 13, mediante a formalização do convênio com a Secretaria de Saúde, para atuar como Responsáveis Técnicos apenas na fase clínica de órteses customizadas.

---

### 4.6. Viabilidade Legal da Logística Reversa de Resíduos Industriais

Para mitigar custos com a aquisição de MDF e acrílico virgem, a parceria com as empresas do distrito industrial de Vinhedo será amparada legalmente conforme o ordenamento jurídico vigente:

1.  **Fundamentação Tributária de Isenção (RICMS-SP):**
    *   A saída de resíduos industriais em formato de aparas, sucatas ou retalhos sob a classificação de resíduos sólidos comuns goza do diferimento ou isenção da incidência do ICMS no Estado de São Paulo, conforme dispõe o **Artigo 392 do Regulamento do ICMS (RICMS/00 - Decreto Estadual nº 45.490/2000)**.
    *   As indústrias emitirão Nota Fiscal de Baixa de Ativo ou Doação de Resíduos Sólidos sob o **CFOP 5.910 (Remessa em doação)** ou **5.949 (Outra saída de mercadoria não especificada)**, descrevendo a mercadoria como "Retalhos e sobras de MDF/Acrílico para fins de aproveitamento municipal em educação inclusiva", sem ônus fiscal para o doador.
2.  **Instrumento de Doação Municipal:**
    *   A prefeitura emitirá, por meio da Secretaria Municipal de Educação, o **Termo de Recebimento de Doação de Bens Móveis Inservíveis**, atestando o recebimento da carga e integrando-a ao almoxarifado do laboratório. Esse documento formal serve de lastro para as auditorias patrimoniais do Controle Interno e do TCE-SP, eliminando qualquer indício de favorecimento ou irregularidade administrativa.
3.  **Outorga do Selo "Empresa Parceira da Inclusão":**
    *   Regulado por Decreto Executivo, o selo certificará as empresas que comprovarem a destinação sistemática de insumos viáveis ao laboratório (meta mínima anual de $200\text{ kg}$ de MDF/acrílico).
    *   A certificação confere à empresa doadora o direito de exploração comercial do selo em suas embalagens, mídias institucionais e relatórios ESG, evidenciando sua responsabilidade social e engajamento com a causa da educação inclusiva e do desenvolvimento tecnológico em Vinhedo/SP.
