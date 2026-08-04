# User Stories — Sistema de Investimentos

### US01 — Cadastro da tese de investimento
**Como** investidor
**Quero** cadastrar os critérios da minha tese de investimento
**Para** que o sistema tome decisões de alocação seguindo exatamente esses critérios

**Critérios de Aceite (BDD)**
- Given que estou na tela de configuração da tese
- When defino os critérios (ativos elegíveis, pesos, limites por categoria)
- Then o sistema salva a tese e passa a usá-la em todos os cálculos futuros

---

### US02 — Importação automática da carteira
**Como** investidor
**Quero** que meus investimentos realizados na corretora subam automaticamente para o sistema
**Para** não precisar atualizar minha carteira manualmente

**Critérios de Aceite (BDD)**
- Given que realizei uma compra de ativo na corretora
- When a integração é sincronizada
- Then o ativo aparece automaticamente consolidado na minha carteira no sistema

---

### US03 — Cálculo automático de rebalanceamento
**Como** investidor
**Quero** informar o valor de um novo aporte e receber a distribuição recomendada
**Para** investir seguindo minha tese, sem decisão manual no momento

**Critérios de Aceite (BDD)**
- Given que tenho uma tese de investimento cadastrada e a carteira consolidada
- When informo o valor do aporte
- Then o sistema calcula e exibe a distribuição recomendada entre os ativos

---

### US04 — Acompanhamento visual da carteira
**Como** investidor
**Quero** visualizar gráficos da composição e evolução da minha carteira
**Para** acompanhar a performance sem depender de um consolidador externo pago

**Critérios de Aceite (BDD)**
- Given que tenho ativos consolidados no sistema
- When acesso a tela de acompanhamento
- Then vejo gráficos de composição atual e evolução histórica da carteira
