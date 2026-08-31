# 🏢 Projeto Integrador: Gestão de Dados e Estrutura Organizacional

> Trabalho acadêmico da disciplina de Gestão de Dados focado no planejamento estratégico de uma organização e na governança de seu ecossistema de software e dados.

---

## 👥 Equipe e Divisão de Responsabilidades

| Membro | Cargo na Empresa (Vitalis Saúde Digital) | Atribuição no Projeto GitHub |
| :--- | :--- | :--- |
| **Carlos Henrique Santiago** | CEO (Diretor Executivo) | Líder do Repositório & Identidade Institucional |
| **João Guilherme Pinheiro** | CMO / Diretor Comercial | Produtos, Serviços e Ecossistema de Parceiros |
| **Joalisson Pinto Maia** | COO (Diretor de Operações) | Organograma e Processos de Negócio |
| **Hudnei Sued Santana** | Arquiteto de Software | Escopo da Plataforma e Ciclo de Dados |
| **Gustavo Bezerra Nonato** | Engenheiro / DBA de Dados | Infraestrutura de Banco e Armazenamento em Nuvem |
| **Mateus Queiroz** | DPO (Encarregado LGPD / Segurança) | Proteção de Dados Sensíveis e Criptografia |
| **Emerson Lucas Sacramento** | Analista de Governança e Riscos | Análise de Riscos de Dados e Valor de Negócio |

# PARTE 1: MODELAGEM DA EMPRESA

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 1                                    -->
<!-- ======================================================== -->
## 1.1 Identidade Institucional
*Responsável: [Nome do Integrante 1]*

### 1.1.1 Nome da Empresa e Marca
* **Nome Fantasia:** [Inserir nome aqui]
* **Razão Social:** [Inserir razão social aqui]
* **Justificativa da Marca:** [Descrever o significado e a proposta do nome]

### 1.1.2 Segmento de Atuação
* [Definir nicho de mercado, área de atuação e modelo de negócio (ex.: B2B, B2C, SaaS)]

### 1.1.3 Missão, Visão e Valores
* **Missão:** [Propósito fundamental e razão de existir da empresa]
* **Visão:** [Onde a organização almeja chegar a médio/longo prazo]
* **Valores:**
  * *[Valor 1]:* [Breve descrição]
  * *[Valor 2]:* [Breve descrição]
  * *[Valor 3]:* [Breve descrição]
  * *[Valor 4]:* [Breve descrição]

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 2                                    -->
<!-- ======================================================== -->
## 1.2 Mercado, Oferta e Ecossistema
*Responsável: [Nome do Integrante 2]*

### 1.2.1 Produtos e Serviços
* [Listar e detalhar o portfólio de produtos e serviços oferecidos ao mercado]

### 1.2.2 Clientes
* [Mapear o público-alvo, personas e perfil dos clientes atendidos]

### 1.2.3 Fornecedores e Parceiros Estratégicos
* [Identificar fornecedores críticos (infraestrutura, insumos, telecomunicações) e parceiros de negócio]

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 3                                    -->
<!-- ======================================================== -->
## 1.3 Estrutura Organizacional e Estratégia
*Responsável: [Nome do Integrante 3]*

### 1.3.1 Organograma
* [Apresentar a estrutura hierárquica e departamental em formato de lista, tabela ou diagrama Mermaid]

### 1.3.2 Principais Processos de Negócio
* [Descrever os macroprocessos operacionais, de gestão e de suporte da organização]

### 1.3.3 Objetivos Estratégicos
* [Listar metas estratégicas mensuráveis de curto, médio e longo prazo (ex.: OKRs/KPIs)]

---

# PARTE 2: PROJETO DE SOFTWARE E GESTÃO DE DADOS

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 4                                    -->
<!-- ======================================================== -->
## 2.1 Visão Geral do Software e Ciclo de Dados
*Responsável: [Nome do Integrante 4]*

### 2.1.1 Descrição do Sistema / Produto de Software
* [Apresentar o software da empresa: proposta, finalidade e escopo funcional]

### 2.1.2 Dados Produzidos e Utilizados
* **Dados de Entrada / Produzidos:** [Dados gerados pela operação do software]
* **Dados Utilizados / Consumidos:** [Bases de dados consultadas, integrações de entrada]

### 2.1.3 Atores e Utilização dos Dados
* [Mapear quem consome ou manipula cada tipo de dado (usuários finais, áreas internas, sistemas parceiros)]

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 5                                    -->
<!-- ======================================================== -->
## 2.2 Arquitetura de Armazenamento
*Responsável: Joalisson Pinto Maia*

### 2.2.1 Onde os Dados são Armazenados

Para atender à demanda da **Vitalis Saúde Digital**, adota-se o conceito de **Persistência Poliglota** (*Polyglot Persistence*), utilizando o banco de dados adequado para cada tipo de dado operacional, clínico ou transacional:

* **Bancos de Dados Relacionais (PostgreSQL):**
  * **Aplicação:** Armazenamento de dados altamente estruturados que exigem conformidade ACID (Atomicidade, Consistência, Isolamento e Durabilidade).
  * **Conteúdo:** Prontuário Eletrônico do Paciente (PEP), históricos de consultas, prescrições médicas, cadastro de usuários (médicos e pacientes), agendamentos e transações financeiras.
* **Bancos de Dados NoSQL / Orientados a Documentos (MongoDB / DynamoDB):**
  * **Aplicação:** Armazenamento de dados semiestruturados de alta velocidade de escrita e leitura sem esquema fixo.
  * **Conteúdo:** Logs de auditoria e acesso à plataforma (*audit logs* para rastreamento de quem acessou dados de saúde), sessões ativas de telemedicina e telemetria capturada de dispositivos *wearables*.
* **Armazenamento de Objetos em Nuvem (AWS S3 / Azure Blob Storage):**
  * **Aplicação:** Armazenamento de dados não estruturados de grande porte com alta durabilidade.
  * **Conteúdo:** Exames laboratoriais, laudos radiológicos e diagnósticos por imagem (formatos PDF, DICOM, JPEG/PNG), além de gravações e transcrições de teleconsultas.
* **Camada de Cache em Memória (Redis):**
  * **Aplicação:** Armazenamento temporário em memória de baixíssima latência.
  * **Conteúdo:** Sessões de login, agendas de médicos disponíveis no dia e tokens de autenticação temporários.

---

### 2.2.2 Infraestrutura de Nuvem Selecionada

A infraestrutura é 100% baseada em nuvem, selecionando a **AWS (Amazon Web Services)** (com possibilidade de contingência na **Microsoft Azure**) para garantir **Alta Disponibilidade (HA)**, tolerância a falhas e total conformidade com a LGPD no que tange à soberania dos dados:

* **Região Geográfica de Alocação:** Datacenters localizados na **Região Brasil (São Paulo - sa-east-1)**, garantindo menor latência para as teleconsultas e conformidade legal na guarda de dados em território nacional.
* **Arquitetura Multi-AZ (Múltiplas Zonas de Disponibilidade):** 
  * Os bancos de dados relacionais (PostgreSQL gerenciado via AWS RDS) operam em configuração *Primary / Standby* replicados de forma síncrona em zonas fisicamente distintas. Em caso de queda de um datacenter, o *failover* é automático.
* **Escalabilidade Automática (Auto Scaling) e Balanceamento de Carga (ALB):** 
  * A camada de aplicação e os serviços de armazenamento se ajustam automaticamente de acordo com o tráfego de acesso e pico de consultas no sistema.

---

### 2.2.3 Política de Retenção, Rotinas de Backup e Ciclo de Vida dos Dados Médicos

A gestão do ciclo de vida dos dados na Vitalis obedece às normas vigentes da área da saúde, em especial à **Lei nº 13.787/2018** (Guarda e Manuseio de Prontuários Eletrônicos) e à **LGPD**:

#### 2.2.4. Rotinas de Backup e Plano de Contingência
* **Backups do Banco Relacional (PostgreSQL / RDS):**
  * **Point-In-Time Recovery (PITR):** Snapshots contínuos das transações permitindo a restauração do banco de dados para qualquer segundo exato dos últimos 35 dias.
  * **Backups Diários e Semanais:** Cópias diárias incrementais e semanais completas encriptadas em repositório secundário isolado.
* **Métricas de Recuperação (SLA/DRP):**
  * **RPO (Recovery Point Objective):** < 5 minutos (perda máxima aceitável de dados em caso de desastre).
  * **RTO (Recovery Time Objective):** < 1 hora (tempo máximo para restabelecimento total dos serviços).

#### 2.2.5. Política de Retenção Legal de Dados Médicos
* **Prontuários e Dados Clínicos:** Guardados obrigatoriamente pelo prazo mínimo de **20 (vinte) anos** a partir do último registro do paciente, conforme determinação legal da Lei 13.787/2018.
* **Logs de Acesso e Auditoria:** Mantidos por no mínimo **6 (seis) meses** para atender aos requisitos do Marco Civil da Internet e diretrizes da LGPD.

#### 2.2.6. Ciclo de Vida do Armazenamento (Storage Lifecycle Rules)
Para otimizar custos e manter a conformidade legal, os arquivos e documentos médicos em formato não estruturado (S3 Buckets) transitam por três camadas automatizadas:

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 6                                    -->
<!-- ======================================================== -->
## 2.3 Privacidade e Proteção de Dados Sensíveis
*Responsável: [Nome do Integrante 6]*

### 2.3.1 Mapeamento de Dados Sensíveis
* [Identificar dados pessoais sensíveis conforme a LGPD e regulamentações do setor]

### 2.3.2 Mecanismos de Segurança e Privacidade
* [Protocolos de criptografia (em trânsito e em repouso), mascaramento/anonimização e controle de acesso (RBAC)]

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 7                                    -->
<!-- ======================================================== -->
## 2.4 Governança, Riscos e Valor de Negócio
*Responsável: [Nome do Integrante 7]*

### 2.4.1 Problemas Relacionados aos Dados
* [Mapear desafios de qualidade dos dados (duplicidade, inconsistência, latência, erros de preenchimento)]

### 2.4.2 Riscos Identificados
* [Riscos operacionais, de indisponibilidade, vazamento e sanções regulatórias]

### 2.4.3 Necessidades do Negócio
* [Como o gerenciamento e a arquitetura de dados atendem às dores estratégicas e operacionais da organização]

---
