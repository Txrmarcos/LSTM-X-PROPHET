
# Análise Comparativa entre LSTM e Prophet - Atualizada

## Resultados Obtidos

### Métricas de Desempenho

* **Modelo LSTM** :
  * **RMSE** : 78.71
* **Modelo Prophet** :
  * **RMSE** : 22.4304

## Discussão das Métricas

O RMSE (Root Mean Square Error) foi a métrica escolhida para avaliar o desempenho dos modelos. Esta métrica é particularmente útil porque:

1. **Interpretabilidade** : O RMSE está na mesma unidade da variável-alvo, facilitando a interpretação direta do erro.
2. **Sensibilidade a outliers** : Como eleva os erros ao quadrado antes de calcular a média, dá mais peso a erros grandes.
3. **Comparabilidade** : Permite comparação direta entre diferentes modelos.

Segundo Hyndman & Koehler (2006), o RMSE é uma das métricas mais adequadas para comparar desempenho de modelos de previsão.

## Análise Comparativa Atualizada

1. **Desempenho** : O modelo Prophet apresenta melhor desempenho (RMSE de 22.4304).
2. **Interpretação dos valores** :

* O RMSE do Prophet (22.43) indica que, em média, as previsões erram por ~22 unidades
* O RMSE do LSTM (78.71) mostra erros aproximadamente 3.5 vezes maiores

## Conclusão

* O modelo Prophet demonstrou melhor desempenho para este conjunto de dados específico
* O LSTM requer mais ajuste de hiperparâmetros e pode ser mais complexo de implementar
* Prophet geralmente performa melhor com padrões sazonais claros
* LSTMs podem capturar padrões complexos mas requerem mais dados e tuning

 **Referência** :
Hyndman, R. J., & Koehler, A. B. (2006). "Another look at measures of forecast accuracy". International Journal of Forecasting, 22(4), 679-688
