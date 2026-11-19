# Análise da Demanda de Ônibus em São Paulo (2019–2026) 🚌

## Sobre o projeto

Este projeto foi desenvolvido para a disciplina de Microeconomia, com o objetivo de analisar a demanda pelo transporte público por ônibus no município de São Paulo e sua relação com as alterações tarifárias entre janeiro de 2019 e agosto de 2026.

O estudo aborda conceitos relacionados à demanda, aos bens substitutos e às externalidades na mobilidade urbana, utilizando técnicas de Ciência de Dados para organizar e explorar informações históricas da SPTrans.

## Objetivos

- Analisar a evolução mensal da quantidade de passageiros transportados e pagantes.
- Integrar informações sobre a demanda e as tarifas municipais.
- Calcular indicadores de variação mensal e interanual.
- Identificar comportamentos atípicos na série histórica.
- Preparar dados estruturados para visualização no Power BI.

## Tecnologias utilizadas

- **Python:** desenvolvimento do processamento de dados.
- **Pandas:** limpeza, transformação, consolidação e análise.
- **NumPy:** operações numéricas e validação de indicadores.
- **Matplotlib:** construção de gráficos.
- **Google Colab:** ambiente de desenvolvimento.
- **Google Drive:** armazenamento dos arquivos.
- **Excel e CSV:** formatos de entrada e saída.
- **Power BI:** ferramenta prevista para visualização dos resultados.

## Etapas do projeto

### 1. Coleta e exploração dos dados

Foram reunidas 92 planilhas mensais da SPTrans, referentes ao período de janeiro de 2019 a agosto de 2026.

A exploração inicial permitiu identificar diferenças nos cabeçalhos, na estrutura das tabelas e na organização dos registros.

### 2. Limpeza e padronização

Foram desenvolvidos procedimentos para padronizar os nomes das colunas, identificar os períodos e tratar registros que poderiam comprometer a consolidação, como linhas de totais gerais e arquivos duplicados.

### 3. Consolidação das informações

Após o tratamento, foram organizados dois conjuntos principais:

- **Base detalhada:** 124.749 registros por linha de ônibus.
- **Base mensal:** 92 observações consolidadas, contendo passageiros transportados e pagantes.

### 4. Integração das tarifas

Foram incorporados os valores históricos das tarifas municipais de ônibus. Nos meses com reajustes, foi calculada uma média ponderada pelos dias de vigência de cada valor.

Essa variável representa uma referência tarifária nominal, e não o preço médio efetivamente pago pelos passageiros.

### 5. Indicadores econômicos

Foram calculados indicadores como:

- Variação percentual mensal da demanda.
- Variação percentual mensal da tarifa.
- Variação interanual de passageiros transportados.
- Variação interanual de passageiros pagantes.
- Participação percentual dos passageiros pagantes.

### 6. Validação e análise de anomalias

Foram realizadas verificações de duplicatas, períodos ausentes e consistência dos cálculos.

Uma ocorrência relevante foi identificada em maio de 2025, quando houve uma redução de aproximadamente 34,01% na quantidade de passageiros transportados em comparação com abril.

Como a causa dessa redução não foi confirmada, o registro foi preservado e classificado como **Em investigação**.

### 7. Exportação

Os dados tratados foram exportados em arquivos CSV e Excel para permitir sua utilização em ferramentas de visualização e análise.

## Resultados do processamento

| Indicador | Resultado |
|---|---|
| Período analisado | Jan/2019 a Ago/2026 |
| Planilhas processadas | 92 |
| Registros detalhados | 124.749 |
| Observações mensais | 92 |
| Meses ausentes | 0 |
| Divergências na consolidação | 0 |
| Registros mensais sob investigação | 1 |

## Limitações

A análise da demanda e das tarifas permite identificar variações e padrões históricos, mas não é suficiente, isoladamente, para comprovar relações de causa e efeito.

Da mesma forma, a substituição entre ônibus e aplicativos de transporte e os efeitos sobre congestionamentos exigiriam informações complementares para uma avaliação quantitativa.

## Fontes de dados

- SPTrans — Dados mensais de passageiros do transporte público por ônibus.
- Prefeitura de São Paulo — Histórico das tarifas municipais.

## Contexto acadêmico

Projeto desenvolvido na disciplina de Microeconomia do curso de **Ciência de Dados e Inteligência Artificial**, da Universidade Federal de Santa Maria (UFSM), campus Cachoeira do Sul.

**Área:** Ciência de Dados, Análise de Dados e Microeconomia.
