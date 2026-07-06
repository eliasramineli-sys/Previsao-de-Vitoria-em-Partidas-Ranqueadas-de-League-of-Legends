# Previsão de Vitória em Partidas Ranqueadas de League of Legends

## Visão Geral

Este projeto tem como objetivo prever se o **time azul vencerá uma partida ranqueada de League of Legends**, utilizando dados estatísticos dos primeiros minutos da partida.

O projeto aplica um fluxo completo de Ciência de Dados, incluindo análise exploratória, engenharia de atributos, treinamento de modelos, ajuste de hiperparâmetros, avaliação de desempenho e interpretação dos resultados para stakeholders.

---

## Problema de Negócio

Em partidas competitivas, pequenas vantagens nos primeiros minutos podem influenciar diretamente o resultado final.
Este projeto busca responder:

> É possível prever a vitória do time azul com base nas estatísticas iniciais da partida?

---

## Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* XGBoost
* Jupyter Notebook
* Streamlit
* Joblib

---

## Estrutura do Projeto

```bash
projeto-lol/
│
├── notebooks/
│   └── Previsao_Vitoria_LOL.ipynb
│
├── imagens/
│   ├── distribuicao_alvo.png
│   ├── heatmap_correlacao.png
│   ├── comparacao_modelos_auc.png
│   ├── curva_roc.png
│   ├── matriz_confusao.png
│   ├── importancia_variaveis.png
│   └── app_streamlit.gif
│
├── modelo/
│   ├── modelo_lol_vitoria_blue.pkl
│   └── colunas_modelo_lol.pkl
│
├── app.py
├── requirements.txt
└── README.md
```

---

## Etapas do Projeto

1. Carregamento da base de dados
2. Análise exploratória dos dados
3. Visualização da variável alvo
4. Análise de correlação
5. Engenharia de atributos
6. Separação entre treino e teste
7. Treinamento de múltiplos modelos
8. Ajuste de hiperparâmetros
9. Avaliação com AUC, F1-score, matriz de confusão e curva ROC
10. Interpretação dos resultados para stakeholders
11. Deploy simples com Streamlit

---

## Visualizações do Projeto

### Distribuição da Variável Alvo

![Distribuição da variável alvo](imagens/distribuicao_alvo.png)

A variável alvo apresentou distribuição equilibrada entre vitórias e derrotas, o que contribui para um treinamento mais justo dos modelos.

---

### Heatmap de Correlação

![Heatmap de correlação](imagens/heatmap_correlacao.png)

O heatmap ajuda a identificar quais variáveis possuem maior relação com a vitória do time azul.

---

### Comparação dos Modelos por AUC

![Comparação dos modelos AUC](imagens/comparacao_modelos_auc.png)

A métrica AUC foi usada para comparar a capacidade dos modelos em diferenciar vitórias e derrotas.

---

### Curva ROC

![Curva ROC](imagens/curva_roc.png)

A Curva ROC mostra que o modelo final possui boa capacidade de classificação.

---

### Matriz de Confusão

![Matriz de confusão](imagens/matriz_confusao.png)

A matriz de confusão apresenta os acertos e erros do modelo, facilitando a interpretação do desempenho.

---

### Importância das Variáveis

![Importância das variáveis](imagens/importancia_variaveis.png)

As variáveis mais importantes indicam quais fatores mais influenciaram as previsões do modelo.

---

## Demonstração do Aplicativo

![Demonstração do app](imagens/app_streamlit.gif)

O aplicativo em Streamlit permite carregar dados e visualizar a probabilidade de vitória do time azul.

---

## Modelos Testados

* Regressão Logística
* Naive Bayes
* Árvore de Decisão
* Random Forest
* Gradient Boosting
* XGBoost
* Voting Classifier

---

## Métricas de Avaliação

As principais métricas utilizadas foram:

* Acurácia
* Precisão
* Recall
* F1-score
* AUC
* Log Loss
* Matriz de Confusão
* Curva ROC

---

## Resultado Final

O modelo final apresentou bom desempenho, com AUC aproximada de **0,81**, demonstrando boa capacidade de diferenciar partidas vencidas e perdidas pelo time azul.

Os principais fatores associados à vitória foram:

* vantagem de ouro;
* controle de objetivos;
* vantagem de experiência;
* diferença de desempenho entre os times.

---

## Como Executar o Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/projeto-lol.git
cd projeto-lol
```

### 2. Crie um ambiente virtual

```bash
python -m venv venv
```

### 3. Ative o ambiente virtual

No Windows:

```bash
venv\Scripts\activate
```

No Linux/Mac:

```bash
source venv/bin/activate
```

### 4. Instale as dependências

```bash
pip install -r requirements.txt
```

### 5. Execute o notebook

```bash
jupyter notebook
```

### 6. Execute o aplicativo Streamlit

```bash
streamlit run app.py
```

---

## Arquivo requirements.txt

```txt
pandas
numpy
matplotlib
scikit-learn
xgboost
streamlit
joblib
jupyter
```

---

## Conclusão

O projeto demonstrou que é possível prever a vitória do time azul em partidas ranqueadas de League of Legends utilizando técnicas de Machine Learning.

Além da boa performance preditiva, o projeto também apresenta interpretações voltadas para stakeholders, tornando os resultados mais compreensíveis e úteis para tomada de decisão.

---

## Próximos Passos

* Implementar explicabilidade com SHAP ou LIME
* Melhorar o deploy com interface mais completa
* Testar LightGBM e CatBoost
* Criar pipeline completo de Machine Learning
* Publicar o app no Streamlit Cloud

---

## Autor

Desenvolvido por **Elias da Silva Santos Filho**

Projeto criado para fins acadêmicos e composição de portfólio profissional em Ciência de Dados.
