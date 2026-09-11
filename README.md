# 📈 ETF Global Investor — EUA + Mundo

## 📌 Sobre o projeto

Este projeto foi desenvolvido como parte do Desafio de Projeto da DIO, utilizando o NotebookLM como ferramenta de aprendizagem ativa, pesquisa, curadoria de fontes e organização do conhecimento.

O tema escolhido foi **ETFs (Exchange Traded Funds)**, com foco em ETFs que proporcionam exposição às maiores empresas dos Estados Unidos e do mercado global.

O projeto busca demonstrar como a Inteligência Artificial pode ser utilizada não apenas para gerar respostas, mas como uma ferramenta de apoio ao estudo, análise crítica, comparação de informações e tomada de decisão baseada em fontes.

---

## 🎯 Contexto e objetivos

O mercado de ETFs possui milhares de produtos diferentes, com características, índices, custos, estratégias, níveis de risco e exposições geográficas distintas.

Diante dessa complexidade, o objetivo deste Caderno Temático é criar uma estrutura organizada para estudar e comparar ETFs de forma sistemática.

### Objetivos principais

* Compreender o funcionamento dos ETFs;
* Entender as principais características de um ETF;
* Comparar ETFs dos Estados Unidos e globais;
* Analisar custos, diversificação e concentração;
* Compreender conceitos como TER, tracking difference, AUM e replicação;
* Estudar indicadores de risco e desempenho;
* Analisar a concentração em grandes empresas;
* Investigar a sobreposição entre diferentes ETFs;
* Desenvolver prompts reutilizáveis para pesquisas futuras;
* Utilizar o NotebookLM para realizar pesquisas fundamentadas nas fontes selecionadas;
* Desenvolver pensamento crítico sobre as respostas produzidas por Inteligência Artificial.

---

## 🧠 NotebookLM como ferramenta de aprendizagem

O NotebookLM foi utilizado como um ambiente de estudo baseado em fontes.

Em vez de solicitar respostas genéricas à Inteligência Artificial, foram selecionadas fontes específicas e os prompts foram elaborados para orientar a análise dessas fontes.

O processo utilizado foi:

**Curadoria → Upload das fontes → Engenharia de Prompts → Análise → Verificação → Síntese → Miniguia**

A proposta foi utilizar a IA como um **assistente de pesquisa e aprendizagem**, mantendo a validação humana das informações.

---

## 📚 Curadoria de fontes

As fontes foram selecionadas priorizando documentos oficiais, fontes institucionais e plataformas especializadas.

### Fontes principais

1. **Vanguard**

   * Informações sobre ETFs, fundos, índices, custos e características dos produtos.

2. **iShares / BlackRock**

   * Informações oficiais sobre ETFs, índices, composição, custos e metodologia.

3. **Invesco**

   * Informações oficiais sobre ETFs, incluindo produtos relacionados ao Nasdaq-100.

4. **justETF**

   * Plataforma especializada para comparação e análise de ETFs disponíveis no mercado europeu.

5. **Morningstar**

   * Dados e informações para análise e comparação de ETFs.

### Critérios de seleção

As fontes foram escolhidas considerando:

* confiabilidade;
* autoridade da fonte;
* atualidade;
* disponibilidade pública;
* qualidade dos dados;
* relevância para investidores europeus;
* possibilidade de verificação das informações.

---

## 🤖 Engenharia de Prompts

Foram desenvolvidos prompts específicos para transformar o NotebookLM em um assistente de análise de ETFs.

A estratégia foi dividir as perguntas por finalidade:

* análise de mercado;
* comparação de ETFs;
* avaliação de risco;
* valuation;
* concentração;
* sobreposição entre ETFs;
* análise macroeconômica;
* estratégia de investimento;
* análise de quedas;
* identificação de oportunidades;
* revisão de carteira.

O projeto também utiliza um **Prompt Master**, responsável por definir a metodologia geral utilizada nas análises.

---

## 🧪 Testes e "Cicatrizes"

Durante o desenvolvimento dos prompts, algumas dificuldades foram identificadas.

### Problema 1 — Respostas genéricas

Prompts muito amplos produziam respostas pouco úteis.

**Solução:**

Adicionar critérios específicos, estrutura obrigatória e solicitação de evidências nas fontes.

---

### Problema 2 — Confusão entre qualidade e preço

Um ETF ou empresa pode ser excelente, mas estar negociado a uma avaliação elevada.

**Solução:**

Separar explicitamente:

**"É um bom ativo?"**

de

**"É um bom preço para comprar?"**

---

### Problema 3 — Tentativa de prever o melhor momento

Perguntas como "qual é o melhor dia para comprar?" podem induzir a IA a apresentar uma falsa precisão.

**Solução:**

Orientar o modelo a comparar estratégias como:

* investimento imediato;
* DCA;
* compra parcelada;
* espera por correção;
* DCA + aportes extraordinários.

---

### Problema 4 — Concentração escondida

ETFs diferentes podem possuir muitas das mesmas empresas.

Por exemplo, um ETF global e um ETF do S&P 500 podem possuir simultaneamente grandes posições em empresas como NVIDIA, Microsoft, Apple, Amazon e Alphabet.

**Solução:**

Criar prompts específicos para analisar **overlap e concentração**.

---

### Problema 5 — Dados desatualizados

Dados de TER, AUM, holdings, preços e valuation podem mudar.

**Solução:**

Instruir o NotebookLM a indicar quando uma informação não está disponível ou pode estar desatualizada, evitando a criação de dados.

---

## 📊 Miniguia de Estudo

### O que é um ETF?

ETF significa **Exchange Traded Fund**.

É um fundo negociado em bolsa que normalmente procura acompanhar o desempenho de um índice, conjunto de ativos ou estratégia específica.

---

### O que é diversificação?

Diversificação significa distribuir o investimento entre diferentes ativos, empresas, setores ou regiões.

Um ETF global pode oferecer exposição a centenas ou milhares de empresas através de uma única posição.

---

### O que é TER?

**TER — Total Expense Ratio**

Representa os custos anuais correntes do fundo.

Em geral, custos menores são desejáveis quando outros fatores são equivalentes.

---

### O que é AUM?

**Assets Under Management**

Representa o patrimônio administrado pelo fundo.

Um AUM elevado pode ser um indicador de escala e relevância do ETF, embora não seja, sozinho, uma garantia de qualidade.

---

### O que é Tracking Difference?

É a diferença entre o desempenho do ETF e o desempenho do índice que ele procura acompanhar.

Não deve ser confundida simplesmente com o TER.

---

### O que é replicação?

É a forma utilizada pelo ETF para acompanhar seu índice.

Pode ser, por exemplo:

* física;
* otimizada;
* sintética.

---

### O que é Accumulating?

Um ETF **Accumulating (Acc)** reinveste automaticamente os dividendos recebidos pelo fundo.

---

### O que é Distributing?

Um ETF **Distributing (Dist)** distribui os rendimentos aos investidores.

---

### O que é Overlap?

Overlap representa a sobreposição de ativos entre dois ou mais ETFs.

Dois ETFs diferentes podem parecer diversificados, mas possuir muitas das mesmas empresas.

---

## 🔄 Prompts reutilizáveis

### Prompt Master

> Atue como um analista de ETFs, mercados financeiros, empresas e macroeconomia. Analise as informações utilizando prioritariamente as fontes disponíveis neste notebook. Diferencie fatos, análise, hipóteses e previsões. Nunca invente dados. Ao analisar um ETF, considere custos, diversificação, liquidez, composição, concentração, risco, valuation, desempenho e adequação ao longo prazo. Diferencie qualidade do ativo de preço de compra. Quando não houver dados suficientes, informe explicitamente essa limitação. Priorize análises que ajudem a construir uma estratégia disciplinada, diversificada, de baixo custo e adequada ao longo prazo.

### Comparação de ETFs

> Compare os ETFs selecionados considerando índice, ISIN, TER, replicação, distribuição, número de holdings, concentração, exposição geográfica, exposição setorial, liquidez, risco, desempenho e adequação para longo prazo. Apresente uma tabela comparativa e indique vantagens e desvantagens de cada ETF.

### Análise de queda

> Analise a queda do ETF. Identifique as possíveis causas, diferencie fatores macroeconômicos de alterações fundamentais e avalie se a queda representa uma correção, crise de mercado, deterioração dos fundamentos ou possível oportunidade de valuation.

### Overlap

> Analise a sobreposição entre os ETFs selecionados. Identifique as principais empresas presentes simultaneamente nos fundos, estime o nível de concentração e explique quais riscos adicionais podem surgir dessa sobreposição.

### Estratégia de aporte

> Compare investimento imediato, DCA, compra parcelada e espera por correção. Analise vantagens, riscos e possíveis limitações de cada estratégia sem afirmar que é possível prever o melhor momento do mercado.

---

## 💡 Principais aprendizados

O desenvolvimento deste projeto mostrou que a qualidade da resposta de uma Inteligência Artificial depende significativamente da qualidade das perguntas, das fontes utilizadas e dos critérios estabelecidos.

Os principais aprendizados foram:

1. IA não substitui a validação das fontes;
2. Prompts específicos produzem respostas mais úteis;
3. Dados financeiros precisam de contexto e data;
4. Diversificação aparente pode esconder concentração;
5. Um ativo de qualidade não é necessariamente uma boa compra em qualquer preço;
6. Não é possível garantir o melhor momento para investir;
7. DCA pode ajudar a reduzir a dependência de decisões de timing;
8. A utilização de fontes primárias aumenta a confiabilidade da análise;
9. O pensamento crítico continua sendo essencial mesmo quando se utiliza IA.

---

## 🛠️ Tecnologias e ferramentas

* GitHub
* Markdown
* NotebookLM
* Inteligência Artificial Generativa
* Engenharia de Prompts
* Pesquisa e curadoria de fontes

---

## 📂 Estrutura do repositório

```text
etf-global-investor-notebooklm/
│
├── README.md
├── fontes/
├── prompts/
├── estudos/
└── evidencias/
```

---

## 🚀 Como reproduzir o projeto

1. Criar um notebook no NotebookLM;
2. Adicionar as fontes selecionadas;
3. Configurar as instruções permanentes;
4. Adicionar a biblioteca de prompts;
5. Executar os prompts;
6. Comparar e validar as respostas;
7. Registrar os resultados;
8. Consolidar os aprendizados no miniguia;
9. Publicar a documentação no GitHub.

---

## ⚠️ Limitações

Este projeto possui finalidade educacional.

As análises produzidas pelo NotebookLM ou por qualquer ferramenta de Inteligência Artificial devem ser verificadas nas fontes originais.

Informações sobre preços, holdings, custos, desempenho e valuation podem mudar ao longo do tempo.

O projeto não constitui recomendação financeira individual.

---

## 👨‍💻 Autor

**Osmar Calado**

Projeto desenvolvido para o **Desafio de Projeto DIO — NotebookLM**.
