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

<a href="https://github.com/user-attachments/assets/f6a34671-a374-4035-accb-531c0170cb02" target="_blank">
  <img src="https://github.com/user-attachments/assets/f6a34671-a374-4035-accb-531c0170cb02" width="1280" alt="grafico_comparativo3" />
</a>

<a href="https://github.com/user-attachments/assets/c9b48aac-355a-4f40-be12-47a8ccad4a50" target="_blank">
  <img src="https://github.com/user-attachments/assets/c9b48aac-355a-4f40-be12-47a8ccad4a50" width="1280" alt="grafico_comparativo2" />
</a>

<a href="https://github.com/user-attachments/assets/17ed01aa-8d64-49e0-bcad-cc198e5d45e" target="_blank">
  <img src="https://github.com/user-attachments/assets/17ed01aa-8d64-49e0-bcad-cc198e5d45e" width="1280" alt="grafico_comparativo1" />
</a>
