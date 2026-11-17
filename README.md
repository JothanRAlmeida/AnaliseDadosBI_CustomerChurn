# 📊 Análise de Churn de Clientes — Telecomunicações

Projeto de análise de dados desenvolvido com **Power BI**, com o objetivo de investigar o comportamento de cancelamento (*Customer Churn*) em uma empresa de telecomunicações, identificar segmentos com maiores taxas de churn e fornecer informações relevantes para apoiar estratégias de retenção de clientes.

O projeto contempla o tratamento e a transformação dos dados com Power Query e linguagem M, criação de medidas utilizando DAX e desenvolvimento de um dashboard interativo para análise dos principais indicadores de negócio.

## 🎯 Objetivos do Projeto

Desenvolver uma solução de Business Intelligence capaz de transformar uma base de dados bruta em informações estratégicas para a área de Operações e Retenção.

A análise busca responder às seguintes perguntas:

- Qual é a taxa de churn da empresa?
- Quantos clientes cancelaram e quantos permanecem ativos?
- Quais tipos de contrato apresentam maiores taxas de cancelamento?
- Como o tempo de relacionamento influencia o comportamento de churn?
- Existe diferença na taxa de cancelamento entre clientes que possuem ou não suporte técnico?
- Quais serviços de internet apresentam maiores taxas de churn?
- Quais métodos de pagamento estão associados às maiores taxas de cancelamento?
- Como a faixa de mensalidade está relacionada ao comportamento de cancelamento?

## 🛠️ Tecnologias e Ferramentas

| Tecnologia | Aplicação |
|---|---|
| Power BI | Desenvolvimento do dashboard e visualização dos indicadores |
| Power Query | Extração, transformação e preparação dos dados |
| Linguagem M | Criação de colunas personalizadas e transformação dos dados |
| DAX | Criação de medidas e cálculos dos indicadores de negócio |

## 🔄 Etapas do Projeto

### 1. Preparação e transformação dos dados

A preparação dos dados foi realizada utilizando o Power Query e a linguagem M, com o objetivo de organizar as informações e criar novas variáveis que facilitassem a análise do comportamento dos clientes.

Foram criadas colunas personalizadas para segmentar os clientes em diferentes categorias:

**Faixa de Mensalidade**

Classificação dos clientes de acordo com o valor da mensalidade:

- 0 a 30
- 31 a 60
- 61 a 90
- 91 a 120

**Tipo de Serviço**

Segmentação dos clientes conforme os serviços contratados:

- Somente Telefone
- Somente Internet
- Telefone + Internet

Essas transformações permitiram criar agrupamentos que facilitam a comparação entre diferentes perfis de clientes e suas respectivas taxas de cancelamento.

### 2. Criação de medidas DAX

Foram desenvolvidas medidas utilizando DAX para calcular os principais indicadores de desempenho e permitir análises dinâmicas no dashboard.

**Indicadores de clientes e churn:**

- `Total de Clientes`: quantidade total de clientes distintos.
- `Clientes Cancelados`: quantidade de clientes que cancelaram os serviços.
- `Clientes Ativos`: quantidade de clientes que permanecem na base.
- `Taxa de Churn`: percentual de clientes cancelados em relação ao total de clientes.

As medidas foram utilizadas para construir os indicadores e gráficos, permitindo que as análises sejam atualizadas conforme as interações e os filtros aplicados no relatório.

### 3. Desenvolvimento do Dashboard

Foi desenvolvido um dashboard interativo no Power BI, com foco na apresentação dos principais indicadores de churn e na identificação dos segmentos de clientes com maiores taxas de cancelamento.

#### Página 1 — Visão Geral do Churn

A página inicial apresenta uma visão executiva do cenário de cancelamentos, permitindo acompanhar os principais indicadores e comparar o comportamento de churn entre diferentes características dos clientes.

**Indicadores (KPIs):**

- Total de Clientes
- Total de Clientes Cancelados
- Total de Clientes Ativos
- Taxa de Churn

**Gráficos e análises:**

| Visualização | Objetivo |
|---|---|
| Taxa de Churn por Tipo de Contrato | Comparar as taxas de cancelamento entre contratos mensal, anual e bienal. |
| Taxa de Churn por Tempo de Permanência | Analisar a relação entre o tempo de relacionamento e o cancelamento. |
| Taxa de Churn por Presença de Suporte Técnico | Comparar o comportamento de cancelamento entre clientes com e sem suporte técnico. |
| Taxa de Churn por Tipo de Serviço de Internet | Identificar diferenças entre os serviços de internet contratados. |
| Taxa de Churn por Método de Pagamento | Avaliar as taxas de cancelamento de acordo com o método de pagamento. |
| Taxa de Churn por Faixa de Mensalidade | Investigar o comportamento de cancelamento conforme o valor da mensalidade. |

**Recursos de interatividade:**

- Filtro por tipo de serviço.
- Segmentação por faixa de tempo de permanência.
- Botão para limpar os filtros aplicados.
- Tooltips personalizados para detalhamento dos indicadores por categoria.
- Interação entre os gráficos para exploração dos dados.

## 📈 Principais Resultados e Insights

Com base nos indicadores apresentados no dashboard, foram identificados alguns padrões relevantes:

**Indicadores gerais:**

| Indicador | Resultado |
|---|---:|
| Total de Clientes | 7.043 |
| Clientes Cancelados | 1.869 |
| Clientes Ativos | 5.174 |
| Taxa de Churn | 26,54% |

**1. Tipo de contrato**

Clientes com contratos mensais apresentam uma taxa de churn de 42,71%, significativamente superior às taxas observadas nos contratos anuais (11,27%) e bienais (2,83%).

**2. Suporte técnico**

Clientes sem suporte técnico apresentam taxa de churn de 41,64%, enquanto clientes com suporte técnico apresentam 15,17%.

**3. Serviço de internet**

A fibra óptica apresenta taxa de churn de 41,89%, enquanto o serviço DSL apresenta 18,96%.

**4. Método de pagamento**

O cheque eletrônico apresenta a maior taxa de churn entre os métodos de pagamento analisados, com 45,29%.

**5. Faixa de mensalidade**

As faixas de mensalidade de 61 a 90 e 91 a 120 apresentam as maiores taxas de churn, com 33,91% e 32,78%, respectivamente.

**6. Tempo de relacionamento**

A visualização indica uma tendência de redução da taxa de churn conforme aumenta o tempo de relacionamento do cliente com a empresa, evidenciando a importância de investigar os primeiros meses da jornada do cliente.

> Os resultados representam associações observadas na base analisada e não devem ser interpretados isoladamente como causas dos cancelamentos.

## 💡 Conclusão

O projeto demonstra como ferramentas de Business Intelligence podem transformar dados operacionais em informações relevantes para a tomada de decisão.

A análise permitiu identificar segmentos com maiores taxas de cancelamento, comparar diferentes características dos clientes e construir uma visão estruturada dos indicadores de churn.

Os resultados podem apoiar a identificação de oportunidades de retenção, a priorização de segmentos para investigação e o direcionamento de futuras estratégias de relacionamento com clientes.

## 🚀 Possíveis Melhorias e Evoluções

Como evolução do projeto, algumas análises podem ser incorporadas:

- Análise de participação de cada segmento no volume total de cancelamentos.
- Cruzamento de variáveis para identificação de perfis com maior concentração de churn.
- Análise de Pareto para identificar as categorias que concentram a maior parte das perdas.
- Análise de mensalidade e tempo de permanência por meio de gráficos de dispersão.
- Inclusão de dados históricos para acompanhar a evolução do churn ao longo do tempo.
- Incorporação de informações sobre motivos de cancelamento, reclamações e histórico de atendimento.
- Desenvolvimento de modelos preditivos para identificação de clientes com maior probabilidade de cancelamento.

## 📷 Dashboard

Abaixo está a visualização da página inicial do projeto:

![Dashboard de Análise de Churn](Images/dashboard-churn.png)