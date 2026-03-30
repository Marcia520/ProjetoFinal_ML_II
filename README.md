## 📘 Projeto Final – Machine Learning II  
### Previsão de Inadimplência de Clientes  
#### Autora: Márcia Aparecida Rodrigues de Sousa  

---

### ▶️ Google Colab  
Execute o notebook diretamente no Google Colab:  
[👉 Abrir no Google Colab](https://colab.research.google.com/github/Marcia520/ProjetoFinal_ML_II/blob/main/ProjetoFinal_(3)(2).ipynb)

---

### 📌 Introdução  
Este projeto aplica **Machine Learning** para prever a inadimplência de clientes de cartão de crédito.  
A solução combina:  
- **Modelos supervisionados**: previsão direta de inadimplência.  
- **Modelos não supervisionados (clustering)**: segmentação de clientes para insights estratégicos.  

---

### 📊 Dataset  
- Fonte: [Credit Card Default Dataset – Kaggle](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset)  
- Registros: ~30.000 clientes  
- Variável alvo: **default payment_next_month** (inadimplência no próximo mês)  

---

### ⚙️ Fluxo do Projeto  
1. Importação e análise exploratória dos dados  
2. Pré-processamento (estratificação, padronização)  
3. **Modelagem supervisionada**  
   - Regressão Logística (baseline)  
   - Random Forest  
   - Support Vector Machine (SVM)  
   - Gradient Boosting  
   - AdaBoost  
4. **Modelagem não supervisionada (clustering)**  
   - K-Means  
   - Agglomerative Clustering  
   - DBSCAN  
5. Otimização de hiperparâmetros com GridSearchCV  
6. Avaliação com métricas:  
   - Supervisionados: Recall, F1-Score, ROC-AUC  
   - Não supervisionados: Silhouette, Davies-Bouldin, Calinski-Harabasz  
7. Comparação dos modelos e análise crítica  

---

### 📈 Resultados  

#### Modelos Supervisionados  
- **Random Forest** e **Gradient Boosting** tiveram melhor desempenho em Recall e ROC-AUC.  
- A regressão logística serviu como baseline interpretável.  

#### Modelos Não Supervisionados  
- **K-Means** e **Agglomerative** mostraram clusters razoáveis.  
- **DBSCAN** identificou outliers, mas com separação limitada.  

---

### ▶️ Como Executar Localmente  
```bash
# Clonar repositório
git clone https://github.com/Marcia520/ProjetoFinal_ML_II.git
cd ProjetoFinal_ML_II

# Instalar dependências
pip install -r requirements.txt

# Abrir notebook
jupyter notebook "ProjetoFinal_(3)(2).ipynb"
```

---

### 🚀 Conclusão  
O projeto demonstrou que **Random Forest** e **Gradient Boosting** são os mais eficazes para prever inadimplência.  
Nos modelos não supervisionados, os clusters revelaram padrões úteis para marketing e análise de perfil.  

**Próximos passos**:  
- Testar algoritmos como XGBoost e LightGBM.  
- Incluir variáveis externas e comportamentais.  
- Monitorar continuamente para detectar **data drift**.  

---

👉 Assim, a combinação de **classificação supervisionada** e **clustering exploratório** amplia o valor da solução, oferecendo previsões precisas e insights estratégicos.  

---
