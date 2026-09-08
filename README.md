# Detecção de Anomalias em Transações Financeiras

Projeto desenvolvido para o módulo de Machine Learning da **DIO (Digital Innovation One)**.

## 📌 Objetivo
Identificar fraudes em transações de cartão de crédito utilizando o algoritmo não supervisionado **Isolation Forest**, avaliando o impacto da taxa de contaminação e comparando os resultados com os dados reais.

## 🛠️ Tecnologias Utilizadas
* Python 3
* Pandas & NumPy (Tratamento de dados)
* Scikit-Learn (Isolation Forest, StandardScaler, PCA, Metrics)
* Matplotlib (Visualização de dados)

## 📊 Principais Resultados
Análise do parâmetro `contamination` e o impacto nos Falsos Positivos vs. Fraudes Perdidas:

| Contaminação | Fraudes Capturadas (Recall) | Alarmes Falsos (Falso Positivo) | Fraudes Perdidas (Falso Negativo) |
| :--- | :--- | :--- | :--- |
| **0.0010** | 104 | 181 | 388 |
| **0.0017** | 138 | 347 | 354 |
| **0.0100** | 299 | 2.550 | 193 |

> **Conclusão:** Aumentar a contaminação melhora a captura de fraudes, porém dispara o número de alarmes falsos (bloqueios indevidos).

## 📈 Visualização (PCA 2D)
A redução de dimensionalidade com PCA permitiu comparar lado a lado a **Realidade** vs. a **Previsão do Modelo**:

<a href="https://github.com/user-attachments/assets/521f51fc-6d5b-4a58-a4af-529e102c2044" target="_blank">
  <img width="1280" height="616" alt="grafico_comparativo1" src="https://github.com/user-attachments/assets/521f51fc-6d5b-4a58-a4af-529e102c2044" />
</a>

<a href="https://github.com/user-attachments/assets/ff84e250-16d0-4706-9ba8-4500551cd497" target="_blank">
  <img width="1280" height="616" alt="grafico_comparativo2" src="https://github.com/user-attachments/assets/ff84e250-16d0-4706-9ba8-4500551cd497" />
</a>

<a href="https://github.com/user-attachments/assets/7375d04f-12b1-47b0-bedf-36fb215f5893" target="_blank">
  <img width="1280" height="616" alt="grafico_comparativo3" src="https://github.com/user-attachments/assets/7375d04f-12b1-47b0-bedf-36fb215f5893" />
</a>




