# 📘 Miniguia — Análise de Dados Aplicada à Gestão Financeira

Este guia consolida os conhecimentos de Análise de Dados Aplicada à Gestão Financeira, integrando fundamentos contábeis, ferramentas tecnológicas e raciocínio investigativo para suporte à decisão estratégica.

## 1. Fundamentos Financeiros Essenciais

**Trindade das Demonstrações (BP, DRE, DFC):** Compreensão do Balanço Patrimonial (posição), DRE (desempenho econômico) e Fluxo de Caixa (dinâmica financeira).

**Finalidade:** Fornecer a base histórica e estruturada do negócio.

**Aplicação:** Identificar se a empresa é lucrativa na DRE, mas insolvente no Caixa.

**Análise Vertical e Horizontal:** A primeira mede o peso das contas (estrutura); a segunda, a evolução temporal (tendência).

**Finalidade:** Detectar mudanças na política da empresa e anomalias de crescimento.

**Métodos de Custeio (Absorção, ABC e Padrão):** Técnicas para apropriar gastos aos produtos e processos.

**Finalidade:** Evitar que um produto pareça lucrativo por rateios distorcidos.

**Aplicação:** Usar o Custeio ABC para identificar atividades que não agregam valor e consomem margem.

## 2. O Papel da Análise de Dados no Financeiro

**Análise Exploratória de Dados (AED/EDA):** Investigação inicial para resumir características e descobrir padrões ocultos.

**Finalidade:** Olhar os dados antes de fazer suposições, detectando outliers ou erros de lançamento.

**Aplicação:** Identificar que o aumento da inadimplência está concentrado em uma região específica.

**Suporte à Decisão Proativa:** Transição do registro histórico para o monitoramento em tempo real e antecipação de riscos.

**Finalidade:** Reduzir a incerteza estrutural inerente ao mercado.

## 3. Complementaridade das Ferramentas

**SQL (Extração):** Linguagem padrão para gerenciar bancos de dados relacionais e agrupar grandes volumes de transações.

**Python/Pandas (Tratamento e Exploração):** Motor de processamento que utiliza DataFrames para limpeza, estatística descritiva e cruzamentos complexos.

**Modelagem de Dados (Estrutura):** Organização em tabelas Fato (eventos) e Dimensão (contexto) em um modelo Star Schema.

**Power BI (Visão e Governança):** Tradução de métricas em indicadores visuais e alertas críticos via DAX.

## 4. Principais Indicadores e Análises
 **Liquidez:** Liquidez Corrente (capacidade de pagamento) e Necessidade de Capital de Giro (NCG).

**Rentabilidade:** ROE (retorno aos sócios), EBITDA (eficiência operacional) e Margens.

**Atividade/Ciclos:** Prazo Médio de Recebimento (PMR), Prazo Médio de Pagamento (PMP) e Ciclo Financeiro.

**Geração de Valor:** EVA (Valor Econômico Agregado), que mede se o lucro supera o custo do capital investido.

## 5. Do Problema à Recomendação (Fluxo Investigativo)

### A metodologia profissional segue a lógica:

**FATO:** Identificação do sintoma (ex: saldo de caixa negativo no Mês 3) [Caso TechLog].

**QUEBRA:** Segmentação do indicador por dimensões (cliente, vendedor, produto, prazo).

**INVESTIGAÇÃO:** Uso de estatística (média vs. mediana) e filtros para isolar a causa.

**CAUSA:** Diagnóstico operacional (ex: vendedores dando 100 dias de prazo sem autorização) [Caso TechLog].

**IMPACTO:** Avaliação financeira do desvio (ex: aumento da NCG e do custo financeiro).

**AÇÃO:** Recomendação de ajuste na política de crédito ou renegociação de prazos.

# 6. Competências Desenvolvidas

**Diagnóstico Financeiro:** Capacidade de ler além do lucro e entender a saúde do caixa.

**Pensamento Analítico:** Substituição da intuição por evidências quantitativas extraídas via SQL e Python.

**Comunicação Visual:** Construção de dashboards que orientam decisões e não apenas apresentam números.

---

## A. Glossário de Conceitos Chave

**Capital de Giro Líquido (CCL):** Diferença entre ativo e passivo circulante; a "folga" financeira.

**DAX (Data Analysis Expressions):** Linguagem de fórmulas do Power BI para criar métricas dinâmicas.

**EBITDA:** Lucro antes de juros, impostos, depreciação e amortização; foca na operação pura.

**EVA (Economic Value Added):** Excedente de riqueza criado após pagar o custo de todo o capital utilizado.

**Outlier:** Valor atípico que foge do padrão e pode distorcer a média.

**Tabela Fato:** Tabela central em um modelo de dados que armazena as transações quantitativas (vendas, pagamentos).

## B. 10 Perguntas que um Profissional Orientado por Dados Deve Responder

1- Qual o nosso ciclo financeiro atual e como ele afeta a necessidade de caixa?
2- O aumento do faturamento está gerando lucro operacional (EBITDA) proporcional?
3- Nosso ROI (Retorno sobre Investimento) é superior ao nosso custo de capital (WACC)?
4- Qual a concentração da nossa receita por cliente e qual o risco associado?
5- O lucro apresentado na DRE está se convertendo efetivamente em caixa?
6- Quais produtos estão sendo subsidiados por outros devido a rateios indevidos?
7- Qual o impacto de uma variação de 10% nos custos variáveis sobre o ponto de equilíbrio?
8- Existe correlação direta entre o aumento do prazo de pagamento e o volume de vendas?
9- Nossa liquidez corrente de 1.2 é real ou está inflada por estoques parados?
10- Se a tendência atual de PMR continuar, em quantos meses o caixa ficará negativo?

## C. 5 Prompts Reutilizáveis para Análises Financeiras

"Analise a variação horizontal da receita e do CMV dos últimos 12 meses. Identifique se os custos estão crescendo em velocidade superior à receita e aponte o mês crítico."

"Realize uma quebra (drill-down) das Contas a Receber por vendedor e prazo médio. Isole os vendedores cujos prazos concedidos superam a média em mais de 20%." [Caso TechLog, 93]

"Calcule o Ponto de Equilíbrio considerando custos fixos de [valor] e margem de contribuição de [valor]. Simule cenários com redução de 5% no preço de venda."

"Cruze a tabela de Vendas com a de Recebimentos via SQL. Identifique faturas vencidas há mais de 30 dias por categoria de produto."

"Utilize estatística descritiva (média, mediana e desvio padrão) para avaliar o custo de aquisição de clientes. Identifique outliers que possam indicar gastos ineficientes.
