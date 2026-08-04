# User Stories — Sistema de Gestão de Estoque de Ativos de TI

### US01 — Cadastro de ativo físico
**Como** analista de TI
**Quero** cadastrar um ativo físico (notebook, desktop, monitor)
**Para** ter controle centralizado do inventário

**Critérios de Aceite (BDD)**
- Given que estou na tela de cadastro de ativos
- When preencho tipo, modelo, número de série e status
- Then o ativo é salvo e recebe um QR Code único

---

### US02 — Cadastro de licença de software
**Como** analista de TI
**Quero** cadastrar uma licença de software
**Para** rastrear validade e quantidade de licenças disponíveis

**Critérios de Aceite (BDD)**
- Given que estou na tela de cadastro de ativos não físicos
- When informo nome do software, quantidade de licenças e data de validade
- Then a licença é salva e aparece na listagem de ativos não físicos

---

### US03 — Movimentação de ativo
**Como** analista de TI
**Quero** registrar a movimentação de um ativo para outro colaborador ou área
**Para** manter o histórico de posse sempre atualizado

**Critérios de Aceite (BDD)**
- Given que um ativo está com status "Disponível" ou "Em uso"
- When registro a movimentação para um novo colaborador/área
- Then o sistema atualiza o responsável atual e registra a movimentação no histórico

---

### US04 — Baixa de ativo
**Como** analista de TI
**Quero** dar baixa em um ativo
**Para** removê-lo do inventário ativo quando ele for perdido, danificado ou devolvido ao fornecedor

**Critérios de Aceite (BDD)**
- Given que estou visualizando um ativo
- When seleciono "Dar baixa" e informo o motivo
- Then o status do ativo muda para "Baixado" e ele deixa de aparecer no inventário disponível, mas permanece no histórico

---

### US05 — Consulta via QR Code
**Como** analista de TI
**Quero** escanear o QR Code de um ativo
**Para** consultar rapidamente seus dados e histórico sem precisar buscar manualmente

**Critérios de Aceite (BDD)**
- Given que tenho o QR Code físico de um ativo em mãos
- When escaneio o código
- Then o sistema exibe os dados atuais e o histórico de movimentações do ativo

---

### US06 — Alerta de fim de ciclo de vida
**Como** gestor de TI
**Quero** ser alertado quando um ativo estiver próximo do fim do seu ciclo de vida
**Para** planejar a substituição antes que o equipamento falhe

**Critérios de Aceite (BDD)**
- Given que um ativo está a X dias do fim do seu ciclo de vida estimado
- When essa data se aproxima
- Then o sistema gera um alerta visível para o time de TI

---

### US07 — Relatório de inventário por área
**Como** gestor de área
**Quero** visualizar todos os ativos vinculados à minha equipe
**Para** ter controle sobre os equipamentos sob minha responsabilidade

**Critérios de Aceite (BDD)**
- Given que sou gestor de uma área
- When acesso o relatório de inventário
- Then vejo somente os ativos vinculados à minha área, com status atual de cada um

---

### US08 — Confirmação de devolução no offboarding
**Como** analista de RH
**Quero** consultar todos os ativos vinculados a um colaborador em desligamento
**Para** confirmar que todos foram devolvidos antes de finalizar o processo

**Critérios de Aceite (BDD)**
- Given que um colaborador está em processo de desligamento
- When consulto seu nome no sistema
- Then vejo a lista de todos os ativos ainda vinculados a ele e posso confirmar a devolução de cada um
