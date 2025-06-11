# Previsao_demanda
Este projeto tem como objetivo desenvolver um modelo de previsão de demanda mensal para produtos de uma empresa de manufatura de alcance global. A partir de dados históricos de demanda em diferentes armazéns centrais, busco criar previsões confiáveis para o mês subsequente, auxiliando a empresa a otimizar seu planejamento logístico e de produção.

Contexto

A empresa fornece milhares de produtos distribuídos em dezenas de categorias. Há quatro armazéns centrais responsáveis pela distribuição regional. Como a fabricação acontece em locais distintos ao redor do mundo, o transporte marítimo até os armazéns leva em média mais de um mês. Prever a demanda com precisão para o próximo mês é essencial para reduzir custos de estoque, evitar faltas de produto e melhorar o atendimento ao cliente.

Objetivos do Projeto

Explorar os dados históricos de demanda para entender padrões sazonais, tendências e efeitos especiais (promoções, feriados, etc.).

Pré-processar e limpar o conjunto de dados, tratando valores ausentes, duplicações e variáveis categóricas.

Desenvolver modelos de Machine Learning (ML) adequados para séries temporais e demanda de produtos, como ARIMA, Prophet e modelos baseados em gradient boosting.

Avaliar o desempenho dos modelos usando métricas como MAE (Mean Absolute Error), RMSE (Root Mean Squared Error) e MAPE (Mean Absolute Percentage Error).

Implementar o melhor modelo em um pipeline reproducível, facilitando atualizações mensais das previsões.
