
# 🧪 Testes e Cicatrizes

## Teste 1 — Prompt genérico

### Prompt

"Quais são os melhores ETFs para investir?"

### Resultado

A resposta apresentou vários ETFs, porém sem critérios claros de comparação.

### Problema identificado

O termo "melhor" era subjetivo.

### Melhoria

Passei a especificar critérios:

- custo;
- diversificação;
- liquidez;
- risco;
- concentração;
- valuation;
- horizonte de investimento.

---

## Teste 2 — Introdução de critérios

### Prompt

"Compare os ETFs considerando custo, diversificação, risco e desempenho."

### Resultado

A resposta ficou mais estruturada.

### Problema

Ainda havia pouca distinção entre qualidade do ETF e preço de entrada.

### Melhoria

Foi criada uma regra específica:

"Separe a análise de qualidade do ativo da análise de preço/valuation."

---

## Teste 3 — Controle de alucinação

### Problema

Dados financeiros podem ficar desatualizados.

### Solução

Foi adicionada a instrução:

"Não invente preços, holdings, TER, AUM ou indicadores. Caso os dados não estejam disponíveis nas fontes, informe explicitamente."

### Resultado

A resposta passou a apresentar maior transparência sobre limitações dos dados.
