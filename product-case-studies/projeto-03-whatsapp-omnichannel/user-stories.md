# User Stories — WhatsApp Omnichannel (Robô de Autocontratação)

### US01 — Início automático do atendimento
**Como** cliente que chegou via campanha
**Quero** ser atendido imediatamente ao iniciar a conversa no WhatsApp
**Para** não precisar esperar em fila de atendimento humano

**Critérios de Aceite (BDD)**
- Given que cliquei em um anúncio de campanha e abri o WhatsApp
- When envio a primeira mensagem
- Then o robô inicia o atendimento automaticamente, sem fila de espera

---

### US02 — Autocontratação guiada
**Como** cliente
**Quero** ser guiado passo a passo pelo robô até concluir a contratação
**Para** resolver minha necessidade de crédito sem precisar de um atendente

**Critérios de Aceite (BDD)**
- Given que iniciei o atendimento com o robô
- When forneço os dados solicitados em cada etapa
- Then o robô conduz o fluxo completo até a conclusão da contratação

---

### US03 — Melhor oferta identificada automaticamente
**Como** cliente
**Quero** que o sistema identifique a melhor opção de crédito disponível para mim
**Para** não precisar avaliar manualmente as alternativas

**Critérios de Aceite (BDD)**
- Given que meus dados foram coletados pelo robô
- When o orquestrador processa as opções disponíveis
- Then a melhor oferta é apresentada automaticamente ao cliente

---

### US04 — Transferência para atendente em exceções
**Como** cliente
**Quero** ser transferido para um atendente humano quando o robô não conseguir resolver minha solicitação
**Para** não ficar travado no fluxo automatizado

**Critérios de Aceite (BDD)**
- Given que estou em atendimento com o robô
- When ocorre uma exceção que o robô não consegue tratar
- Then sou transferido automaticamente para um atendente humano
