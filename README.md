<img width="1280" height="616" alt="grafico_comparativo3 (2)" src="https://github.com/user-attachments/assets/f6a34671-a374-4035-accb-531c0170cb02" />
<img width="1280" height="616" alt="grafico_comparativo2 (2)" src="https://github.com/user-attachments/assets/c9b48aac-355a-4f40-be12-47a8ccad4a50" />
<img width="1280" height="616" alt="grafico_comparativo1" src="https://github.com/user-attachments/assets/17ed01aa-8d64-49e0-bcad-cc198e56d45e" />
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

![Comparativo 0.0010 Realidade vs Modelo](grafico_comparativo.png)
![Comparativo 0.0017 Realidade vs Modelo](grafico_comparativo2.png)
![Comparativo 0.0100 Realidade vs Modelo](grafico_comparativo3.png)
