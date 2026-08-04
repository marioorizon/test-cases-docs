# User Stories — Plataforma de Crédito

### US01 — Cadastro do cliente
**Como** cliente em busca de crédito
**Quero** me cadastrar informando meu CPF e dados pessoais
**Para** que a plataforma analise minhas opções de crédito disponíveis

**Critérios de Aceite (BDD)**
- Given que estou na tela de cadastro
- When informo CPF e dados pessoais válidos
- Then meu cadastro é criado e a análise de crédito é iniciada

---

### US02 — Consulta multi-modalidade
**Como** cliente cadastrado
**Quero** que o sistema analise automaticamente todas as modalidades de crédito disponíveis para mim
**Para** não precisar pesquisar em vários bancos ou sites diferentes

**Critérios de Aceite (BDD)**
- Given que meu cadastro foi validado
- When o motor de crédito processa minha análise
- Then recebo o resultado de todas as modalidades para as quais sou elegível (FGTS, antecipação FGTS, consignado CLT, pessoal, garantia de veículo)

---

### US03 — Visualização consolidada das propostas
**Como** cliente
**Quero** visualizar em um único lugar todas as propostas de crédito disponíveis para mim
**Para** comparar e escolher a melhor opção

**Critérios de Aceite (BDD)**
- Given que a análise de crédito foi concluída
- When acesso a tela de propostas
- Then vejo todas as modalidades elegíveis, com valor e condições de cada uma

---

### US04 — Consentimento LGPD
**Como** cliente
**Quero** ser informado e dar meu consentimento sobre o uso dos meus dados
**Para** ter transparência sobre como minhas informações pessoais serão tratadas

**Critérios de Aceite (BDD)**
- Given que estou no fluxo de cadastro
- When chego à etapa de consentimento
- Then devo aceitar explicitamente os termos antes que meus dados sejam usados na análise de crédito

---

### US05 — Seleção de proposta
**Como** cliente
**Quero** selecionar uma das propostas apresentadas
**Para** dar sequência à contratação do crédito

**Critérios de Aceite (BDD)**
- Given que recebi ao menos uma proposta elegível
- When seleciono uma das opções
- Then sou direcionado ao fluxo de contratação daquela modalidade específica
