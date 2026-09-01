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
*Responsável: Carlos Henrique De Souza Santana Santiago*

### 1.1.1 Nome da Empresa e Marca

* **Nome Fantasia:** Vitalis Saúde Digital.

* **Razão Social:** Vitalis Tecnologia em Saúde e Serviços S.A.

* **Justificativa da Marca:**  O nome Vitalis provém do latim vitalis, que significa "pertencente ou relativo à vida", "essencial" e "que sustenta a vida". A junção com Saúde Digital posiciona a organização diretamente no ecossistema de inovação tecnológica, refletindo a proposta de ser uma ponte ágil, segura e vital entre profissionais de saúde e pacientes.

### 1.1.2 Segmento de Atuação

* **Setor:** Tecnologia da Informação aplicada à Saúde (HealthTech).

* **Nicho**: Plataformas integradas de telemedicina, gestão de prontuário eletrônico em nuvem (PEP - Prontuário Eletrônico do Paciente) e emissão de prescrições digitais com assinatura com certificação ICP-Brasil.
  
* **Modelo de Negócio:**
  * B2B (Business to Business): Fornecimento da infraestrutura de software como serviço (SaaS) para clínicas, hospitais de pequeno/médio porte e operadoras de saúde suplementar.
  * B2C (Business to Consumer): Acesso direto de pacientes a consultas eletivas via aplicativo web e mobile.


### 1.1.3 Missão, Visão e Valores
* **Missão:** Democratizar o acesso à saúde de qualidade e humanizada por meio de soluções digitais integradas, conectando pacientes e profissionais de saúde com segurança, eficiência e máxima proteção de dados clínicos.
  
* **Visão:** Consolidar-se como o ecossistema digital de saúde mais confiável do país, unindo telemedicina de ponta e governança avançada de dados clínicos para transformar informações médicas em diagnósticos mais rápidos, precisos e seguros.
  
* **Valores:**
  * ***1 Vida e Saúde em Primeiro Lugar:*** A tecnologia é um meio para salvar vidas e melhorar o cuidado humano; nenhuma decisão técnica ou comercial se sobrepõe ao bem-estar do paciente.
  * ***2 Privacidade e Confidencialidade Inegociáveis:*** Rigor e transparência no tratamento de dados pessoais e clínicos sensíveis, mantendo conformidade contínua com a LGPD e padrões éticos médicos (CFM).
  * ***3 Inovação com Rigor Científico:*** Desenvolvimento de software baseado em evidências, segurança da informação e confiabilidade operacional crítica.
  * ***4 Acessibilidade e Usabilidade:*** Criar experiências digitais intuitivas para que médicos e pacientes — independentemente do nível de letramento digital — tenham uma experiência fluida e sem atritos.]
  * ***5 Integridade e Ética nos Dados:*** Garantia de que diagnósticos, prescrições e laudos sejam imutáveis, rastreáveis e acessíveis apenas por quem tem autorização legítima.

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 2                                    -->
<!-- ======================================================== -->
## 1.2 Mercado, Oferta e Ecossistema
*Responsável: João Guilherme Pinheiro*

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
*Responsável: Gustavo Bezerra Nonato*

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
*Responsável: Hudnei Sued Santana*

### 2.1.1 Descrição do Sistema / Produto de Software
* O VitalisConnect é a plataforma digital de saúde da Vitalis Saúde Digital, responsável por conectar pacientes e profissionais de saúde por meio de teleconsultas, gerenciamento do Prontuário Eletrônico do Paciente (PEP) e emissão de prescrições médicas digitais assinadas com certificado digital.

### 2.1.2 Dados Produzidos e Utilizados

O sistema produz e utiliza diferentes categorias de dados durante o ciclo de atendimento do paciente.

### Dados cadastrais
- Dados de identificação do paciente;
- Informações necessárias para cadastro e identificação.

### Dados clínicos
- Sintomas;
- Anotações de prontuário;
- Histórico clínico;
- Diagnósticos;
- CID-10;
- Informações sobre medicamentos.

### Documentos
- Exames;
- Laudos;
- Prescrições digitais.

### Dados de operação
- Logs de login;
- Registros relacionados ao acesso e utilização do sistema.

### 2.1.3 Ciclo dos Dados

O ciclo de dados do VitalisConnect acompanha o fluxo de atendimento do paciente:

Cadastro → Teleconsulta → Registro no Prontuário → Emissão de Prescrição → Consulta do Histórico e Documentos.

Durante esse fluxo, os dados são produzidos ou atualizados pelos usuários autorizados e posteriormente utilizados para continuidade do atendimento e acesso às informações clínicas.

### 2.1.4 Usuários dos Dados

### Médico/Profissional de Saúde
- Consulta dados do paciente;
- Registra informações no prontuário;
- Consulta histórico clínico;
- Registra diagnósticos;
- Emite prescrições digitais.

### Paciente
- Fornece seus dados cadastrais e informações durante o atendimento;
- Consulta seu histórico;
- Acessa prescrições e documentos relacionados ao atendimento.

### Recepção/Faturamento
- Consulta dados necessários para processos administrativos;
- Utiliza informações relacionadas a pagamento e convênio.

### 2.1.5 Entradas e Saídas

As principais entradas do sistema são os dados cadastrais do paciente, sintomas e informações fornecidas durante a consulta, além dos registros realizados pelos profissionais de saúde.

Como saídas, o sistema disponibiliza o prontuário eletrônico, informações do histórico clínico, documentos relacionados ao atendimento e prescrições médicas digitais.
---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 5                                    -->
<!-- ======================================================== -->
## 2.2 Arquitetura de Armazenamento
*Responsável: Joalisson Pinto Maia*

### 2.2.1 Onde os Dados são Armazenados
* [Definir tipos de bancos de dados (Relacional/SQL, NoSQL, Cache, Object Storage) e ambiente (Nuvem, On-premise, Híbrido)]

### 2.2.2 Estratégia de Persistência e Backup
* [Políticas de retenção de dados, periodicidade de backups e planos de contingência]

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 6                                    -->
<!-- ======================================================== -->
## 2.3 Privacidade e Proteção de Dados Sensíveis
*Responsável: Emerson Lucas Sacramento*

### 2.3.1 Mapeamento de Dados Sensíveis
* [Identificar dados pessoais sensíveis conforme a LGPD e regulamentações do setor]

### 2.3.2 Mecanismos de Segurança e Privacidade
* [Protocolos de criptografia (em trânsito e em repouso), mascaramento/anonimização e controle de acesso (RBAC)]

---

<!-- ======================================================== -->
<!-- SEÇÃO DO INTEGRANTE 7                                    -->
<!-- ======================================================== -->
## 2.4 Governança, Riscos e Valor de Negócio
*Responsável: Mateus Queiroz*

### 2.4.1 Problemas Relacionados aos Dados
* [Mapear desafios de qualidade dos dados (duplicidade, inconsistência, latência, erros de preenchimento)]

### 2.4.2 Riscos Identificados
* [Riscos operacionais, de indisponibilidade, vazamento e sanções regulatórias]

### 2.4.3 Necessidades do Negócio
* [Como o gerenciamento e a arquitetura de dados atendem às dores estratégicas e operacionais da organização]

---
