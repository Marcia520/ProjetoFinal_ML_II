## 📘 Projeto Final – Machine Learning II
### Previsão de Inadimplência de Clientes
#### Autora: Márcia Aparecida Rodrigues de Sousa

### Google Colab

Clique no botão abaixo para abrir e executar o notebook diretamente no Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Marcia520/ProjetoFinal_ML/blob/main/ProjetoFinal%20(3).ipynb)

---

### 📌 Introdução
Este projeto tem como objetivo prever a inadimplência de clientes de cartão de crédito utilizando técnicas de **Machine Learning**.  
A solução foi desenvolvida com base em um dataset público do Kaggle, aplicando um fluxo completo de ML: desde o tratamento dos dados até a comparação de modelos supervisionados e não supervisionados, com otimização e avaliação crítica.

---

### 📊 Dataset
- Fonte: [Credit Card Default Dataset – Kaggle](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset)  
- Registros: ~30.000 clientes  
- Variável alvo: **default payment_next_month** (inadimplência no próximo mês)

---

#### ⚙️ Fluxo do Projeto
1. Importação e análise exploratória dos dados  
2. Pré-processamento (estratificação, padronização)  
3. **Modelagem supervisionada**:
   - Regressão Logística (baseline)
   - Random Forest
   - Support Vector Machine (SVM)
   - Gradient Boosting
   - AdaBoost
4. **Modelagem não supervisionada (clustering)**:
   - K-Means
   - Agglomerative Clustering
   - DBSCAN
5. Otimização de hiperparâmetros com GridSearchCV  
6. Avaliação com métricas Recall, F1-Score e ROC-AUC (supervisionados)  
7. Avaliação com métricas Silhouette, Davies-Bouldin e Calinski-Harabasz (não supervisionados)  
8. Comparação dos modelos e análise crítica da solução  

---

#### 📈 Resultados Obtidos

##### Modelos Supervisionados
| Modelo               | Recall | F1-Score | ROC-AUC |
|----------------------|--------|----------|---------|
| Regressão Logística  | 0.23   | 0.34     | 0.72    |
| Random Forest        | 0.35   | 0.45     | 0.75    |
| SVM                  | 0.28   | 0.38     | 0.73    |
| Gradient Boosting    | 0.33   | 0.44     | 0.76    |
| AdaBoost             | 0.30   | 0.40     | 0.74    |

##### Modelos Não Supervisionados
- **K-Means**: Silhouette ≈ 0.42, Davies-Bouldin ≈ 1.25  
- **Agglomerative Clustering**: Silhouette ≈ 0.40, Davies-Bouldin ≈ 1.30  
- **DBSCAN**: identificou clusters de densidade e alguns outliers, mas com menor separação entre grupos.  

---

### ▶️ Como Executar Localmente

1. Clone este repositório:
   ```bash
   git clone https://github.com/Marcia520/ProjetoFinal_ML.git
   cd ProjetoFinal_ML
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Abra o notebook:
   ```bash
   jupyter notebook "ProjetoFinal (3).ipynb"
   ```

4. Execute célula por célula para reproduzir os resultados.

---

### 🚀 Conclusão
O projeto demonstrou que o **Random Forest** e o **Gradient Boosting** foram os modelos supervisionados mais eficazes para prever inadimplência, com melhor Recall e ROC-AUC.  
Nos modelos não supervisionados, os clusters revelaram padrões interessantes de segmentação, úteis para estratégias de marketing e análise de perfil.  

Para produção, recomenda-se:
- Integração com pipeline de dados.  
- Monitoramento contínuo para detectar **data drift**.  
- Inclusão de variáveis externas e comportamentais.  
- Testes com outros algoritmos de ensemble (XGBoost, LightGBM).  

Assim, a combinação de **classificação supervisionada** e **clustering exploratório** amplia o valor da solução, oferecendo previsões precisas e insights estratégicos.
```

---

