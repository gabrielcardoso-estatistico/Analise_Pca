# Análise Fatorial de Indicadores Municipais 🇧🇷

Este projeto aplica técnicas de estatística multivariada (**AFE** e **PCA**) para identificar os fatores latentes que estruturam o desenvolvimento socioeconômico das cidades brasileiras. O objetivo é reduzir a dimensionalidade de indicadores demográficos e econômicos em dimensões interpretáveis.

## 🛠️ Diagnóstico e Metodologia

Antes da extração dos fatores, os dados foram validados para garantir a adequação da análise:

* **KMO:** 0,84 (Adequação Meritória).
* **Teste de Bartlett:** $p < 0,001$ (Correlações significativas confirmadas).

## 📈 Extração de Componentes

Utilizando o **Critério de Kaiser**, identificamos que **dois componentes** explicam aproximadamente **78,8%** da variância total dos dados. O ponto de inflexão no "Gráfico de Cotovelo" confirma esta decisão:

![Scree Plot](image_c688de.png)

## 📊 Principais Resultados

A análise revelou duas dimensões distintas que regem os municípios:

1. **Porte e Infraestrutura (Dim 1):** Concentra variáveis como PIB Total, Frota de Carros e População.
2. **Desenvolvimento Humano (Dim 2):** Concentra as variáveis de IDHM e PIB per capita.

### Mapa de Variáveis (PCA)
O gráfico abaixo ilustra como as variáveis se agrupam nestas duas dimensões. Note que o porte econômico e o desenvolvimento social são eixos independentes no conjunto de dados.

![Círculo de Correlações](image_c69363.png)

### Contribuição das Variáveis
As variáveis de infraestrutura urbana são as que mais contribuem para a formação do primeiro componente:

![Ranking de Contribuição](image_c6937e.png)

## 🏗️ Estrutura do Modelo
Abaixo, a representação visual de como as variáveis observadas se conectam aos fatores latentes identificados:

![Modelo de Análise Fatorial](esquema.png)

---
*Análise desenvolvida por Gabriel Cardoso.*
