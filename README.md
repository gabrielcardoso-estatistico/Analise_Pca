# Análise Fatorial: Indicadores Municipais Brasileiros 🇧🇷

Este projeto utiliza técnicas de estatística multivariada para identificar dimensões latentes no desenvolvimento dos municípios brasileiros, reduzindo 11 indicadores socioeconômicos em dois fatores principais.

## 🏗️ Modelo Teórico
A análise baseia-se na premissa de que as variáveis observadas (PIB, População, IDHM, etc.) são reflexos de fatores latentes subjacentes. O modelo busca capturar a variância comum entre essas variáveis:

![Modelo de Análise Fatorial](esquema.png)

## 📊 Principais Resultados

Após a validação pelos testes KMO (**0,84**) e Bartlett (**p < 0,001**), a análise de componentes principais (PCA) revelou duas dimensões independentes que explicam **78,8%** da variância total:

1. **Porte e Infraestrutura (Dim 1):** Agrupa variáveis de volume como População, PIB Total e frota de veículos.
2. **Desenvolvimento Humano (Dim 2):** Agrupa os indicadores de IDHM e PIB per capita.

O mapa abaixo ilustra como essas variáveis se comportam: as variáveis de porte econômico estão no eixo horizontal, enquanto as de bem-estar social definem o eixo vertical.

![Mapa de Variáveis - PCA](Rplot.png)

---
**Conclusão:** O estudo demonstra que o porte econômico de uma cidade (tamanho) é uma dimensão independente da sua eficiência em gerar desenvolvimento humano (IDHM), permitindo classificações mais precisas para políticas públicas.

*Análise desenvolvida por Gabriel Cardoso.*
