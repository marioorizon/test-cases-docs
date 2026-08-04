# User Stories — Sales Agent IA

### US01 — Prospecção por categoria
**Como** operador do sistema
**Quero** buscar negócios no Google Maps por categoria
**Para** gerar uma base de leads qualificados para prospecção

**Critérios de Aceite (BDD)**
- Given que defini uma categoria de negócio (ex.: clínicas de saúde)
- When executo a busca
- Then o sistema retorna a lista de negócios encontrados na categoria, com seus dados públicos

---

### US02 — Análise de reputação
**Como** operador do sistema
**Quero** que cada negócio encontrado seja analisado quanto à sua reputação no Google
**Para** priorizar leads com maior potencial de melhoria

**Critérios de Aceite (BDD)**
- Given que um negócio foi encontrado na busca
- When o sistema analisa seu perfil no Google
- Then registra nota, quantidade de avaliações e presença de feedbacks negativos

---

### US03 — Geração e envio automático de proposta
**Como** operador do sistema
**Quero** que uma proposta seja formalizada e enviada automaticamente após a análise
**Para** não precisar montar e enviar propostas manualmente uma a uma

**Critérios de Aceite (BDD)**
- Given que a análise do negócio foi concluída
- When o sistema identifica pontos de melhoria
- Then formaliza a proposta e a envia via WhatsApp (se disponível) e/ou e-mail (se disponível)

---

### US04 — Primeiro atendimento via bot
**Como** cliente prospectado que respondeu à proposta
**Quero** ser atendido imediatamente por um bot
**Para** entender rapidamente a proposta e o orçamento

**Critérios de Aceite (BDD)**
- Given que respondi à proposta recebida
- When inicio a conversa
- Then o bot conduz o atendimento inicial até a apresentação do orçamento

---

### US05 — Transferência para atendimento humano
**Como** cliente que aprovou o orçamento
**Quero** ser atendido diretamente pelo responsável pelo serviço
**Para** dar início à execução do projeto (site, Instagram, marketing digital)

**Critérios de Aceite (BDD)**
- Given que aprovei o orçamento apresentado pelo bot
- When essa aprovação é registrada
- Then o atendimento é transferido para o atendimento humano
