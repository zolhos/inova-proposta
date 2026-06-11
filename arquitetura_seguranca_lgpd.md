# Diretrizes de TI, Proteção de Dados e LGPD - Espaço Inova Vinhedo

Este documento estabelece as regras obrigatórias de segurança da informação, arquitetura de sistemas e governança de dados para o **Espaço Inova Vinhedo**, em estrita conformidade com a Lei Geral de Proteção de Dados Pessoais (LGPD - Lei nº 13.709/2018), com foco na proteção de dados sensíveis de crianças, adolescentes e históricos de saúde escolar (AEE).

---

## 1. Classificação dos Dados Tratados

As operações no laboratório e nos sistemas locais envolvem o processamento de dados classificados em três níveis de sensibilidade:

| Tipo de Dado | Exemplos Práticos | Categoria LGPD | Requisito de Proteção |
| :--- | :--- | :---: | :---: |
| **Dados Pessoais Comuns** | Nome do aluno, data de nascimento, nome dos pais/responsáveis, escola de origem, matrícula municipal. | Art. 5º, I | Acesso restrito a servidores autorizados da educação. |
| **Dados Pessoais Sensíveis** | Laudo médico detalhado, CID (Classificação Internacional de Doenças), diagnósticos psicopedagógicos, anotações de evolução clínica. | Art. 5º, II | Criptografia obrigatória, controle rígido de acesso (segredo profissional). |
| **Dados Técnicos Anonimizados** | Arquivos CAD de adaptadores ergonômicos (STL), desenhos de corte a laser (DXF), códigos-fonte de automações em Javascript/Python. | Art. 12 | **Dados Livres.** Podem ser compartilhados publicamente no repositório aberto. |

---

## 2. Diretrizes de Hospedagem e Infraestrutura de TI

Para evitar vazamentos e garantir a soberania dos dados da prefeitura, fica proibido o uso de servidores, bancos de dados ou nuvens públicas gratuitas ou não auditadas (ex: contas pessoais de Google Drive, planos gratuitos de Firebase ou Airtable) para o armazenamento de prontuários e laudos do AEE.

### 2.1. Nuvem de Governo e Servidores Municipais (Datacenter)
*   **Hospedagem Principal:** Todos os aplicativos internos desenvolvidos pela equipe (ex.: sistemas de triagem, controle de agendamento e evolução pedagógica) deverão ser implantados na infraestrutura de servidores da própria Prefeitura de Vinhedo (Datacenter Municipal on-premise) ou em nuvem governamental (G-Cloud) homologada pelo Departamento de TI municipal.
*   **Bancos de Dados Seguros:** Os bancos de dados (como PostgreSQL ou MongoDB corporativos) devem estar isolados em sub-redes privadas e ser acessíveis apenas por meio de conexões autenticadas do backend, proibindo exposição direta das portas de dados à internet.

### 2.2. Segurança e Criptografia
*   **Trânsito de Dados:** Uso obrigatório de protocolo seguro HTTPS com criptografia TLS 1.3 ativa para todas as aplicações web locais e portais.
*   **Criptografia em Repouso:** Os campos de identificação pessoal e prontuários médicos sensíveis nos bancos de dados devem ser criptografados na camada do banco (*Transparent Data Encryption* - TDE) ou do aplicativo antes da gravação.
*   **Trilhas de Auditoria (Logs):** Registro indelével de logs de sistema (quem leu, alterou, exportou ou deletou registros de AEE) por no mínimo 5 anos, atendendo às exigências regulatórias.

### 2.3. Uso do Ecossistema Institucional (Google Workspace, Google Cloud e Firebase)
Para garantir a entrega ágil de pequenos aplicativos e automações, fica homologado o aproveitamento do ecossistema Google já existente na rede municipal, estendendo-se às ferramentas de desenvolvimento em nuvem, sob as seguintes regras:

*   **Ferramentas Low-Code e Ecossistema Integrado:** É autorizado o uso de plataformas nativas do Google Workspace (como Google AppSheet, Forms e Apps Script) para fluxos de baixa complexidade, armazenando dados lógicos em "Drives Compartilhados" institucionais com permissões gerenciadas centralmente.
*   **Aplicações Web de Pequeno Porte (GCC e Firebase):** Para sistemas que exigem maior customização de interface ou sincronização de dados em tempo real, homologa-se o uso do **Google Cloud Console (GCC)** e do **Firebase** (ex: *Firebase Hosting*, *Cloud Firestore* e *Cloud Functions*). **Regra de Ouro:** Todos os projetos devem ser obrigatoriamente provisionados dentro da *Google Cloud Organization* da Prefeitura, atrelados ao faturamento e à auditoria do município. É expressamente proibida a criação de instâncias do Firebase em contas pessoais de desenvolvedores (`@gmail.com`).
*   **Gestão de Identidade e Controle de Acesso (SSO):** A autenticação de usuários em qualquer aplicativo desenvolvido (seja no AppSheet ou customizado via Firebase Auth) deverá ser realizada exclusivamente por meio do Logon Único (SSO) com as credenciais oficiais (domínio `@edu.vinhedo.sp.gov.br`). O desligamento da conta do servidor no painel central do Workspace revogará imediatamente o seu token de acesso em todos os sistemas do AEE.
*   **Governança e Regras de Segurança (Security Rules):** No caso de uso de bancos de dados NoSQL (como o Firestore), o código-fonte deverá conter regras de segurança estritas (Firestore Security Rules) que bloqueiem acessos públicos de leitura/escrita, garantindo que apenas usuários autenticados sob o domínio institucional tenham acesso aos prontuários e laudos anonimizados. A auditoria global e a política de retenção continuarão sendo geridas centralmente pelo Google Vault e painéis do GCC.

---

## 3. Gestão de Consentimento e Salvaguardas Jurídicas

O tratamento de dados de menores no laboratório exige salvaguardas que formalizam a transparência e a segurança jurídica junto aos órgãos de controle (Procuradoria Municipal e Ministério Público):

### 3.1. Termo de Consentimento Livre e Esclarecido (TCLE) - AEE
Antes do ingresso do aluno do AEE nas atividades de codesign ou de oficinas de média/longa duração no Espaço Inova, os pais ou responsáveis legais devem assinar um TCLE físico ou digital contendo:
*   Finalidade específica do tratamento (ex.: *desenvolvimento e fabricação sob medida de adaptador ergonômico de escrita*).
*   Detalhes de quais dados de saúde serão necessários no processo (laudos, moldagens físicas da mão).
*   Garantia do direito de exclusão e revogação do consentimento a qualquer momento, sem prejuízo ao atendimento pedagógico do aluno na rede regular.

### 3.2. Autorização de Uso de Imagem e Voz
A captação de fotos e vídeos dos atendimentos no laboratório serve exclusivamente para documentação técnica de engenharia assistiva (ex: *verificar o ângulo de preensão do lápis antes e depois do uso do adaptador*) ou divulgação institucional interna da Secretaria de Educação.
*   **Consentimento Separado:** O termo de uso de imagem é independente do TCLE do AEE. Os responsáveis podem recusar o uso de imagem sem afetar o codesign do dispositivo do estudante.
*   Fica vedada a publicação de fotos de rostos de alunos do AEE em redes sociais abertas da prefeitura ou meios de comunicação externos sem a anuência específica e expressa no termo.

### 3.3. Termo de Confidencialidade e Sigilo dos Servidores
Os 4 servidores alocados na equipe de revezamento deverão assinar, no momento da designação ao cargo, um **Termo de Compromisso e Manutenção de Sigilo Profissional**, responsabilizando-se civil e administrativamente pelo dever de confidencialidade sobre os laudos de saúde escolar aos quais terão acesso.

---

## 4. Protocolo de Anonimização para a "Rede Municipal de Tecnologia Assistiva Livre"

Ao disponibilizar as inovações de hardware e software geradas em Vinhedo no GitHub ou em portais públicos de tecnologia assistiva livre, a equipe deve seguir rigorosamente as diretrizes de desassociação de dados:

1.  **Eliminação de Identificadores CAD:** O arquivo digital de modelagem 3D (extensões STL, STEP, OBJ, DXF) não deve conter gravados em baixo ou alto-relevo nomes de alunos, iniciais ou identificações de escolas.
2.  **Renomeação e Codificação de Casos:** Os estudos de caso documentados no repositório público devem usar codinomes ou referências abstratas (ex: *Design 012 - Adaptador de Escrita Ergonômico de Baixo Custo*), removendo qualquer menção ao prontuário real do estudante.
3.  **Remoção de Metadados:** Antes do upload de imagens técnicas dos dispositivos adaptados, os arquivos de imagem (como PNG, JPG) devem ter seus metadados de geolocalização (EXIF) e identificadores de câmera removidos.
