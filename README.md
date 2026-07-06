# 🎮 Previsão de Vitória em Partidas Ranqueadas de League of Legends

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![XGBoost](https://img.shields.io/badge/XGBoost-Boosting-green)
![Status](https://img.shields.io/badge/Status-Concluído-success)
![License](https://img.shields.io/badge/License-MIT-blue)

---

# 📌 Sobre o Projeto

Este projeto utiliza técnicas de **Ciência de Dados** e **Machine Learning** para prever se o **time azul vencerá uma partida ranqueada de League of Legends**, utilizando estatísticas coletadas nos primeiros minutos da partida.

O objetivo é desenvolver um modelo capaz de identificar padrões que influenciam o resultado da partida antes do seu término, auxiliando na tomada de decisões e demonstrando a aplicação prática de algoritmos de classificação.

---

# 🎯 Objetivos

* Analisar estatísticas das partidas.
* Identificar quais atributos possuem maior influência na vitória.
* Comparar diversos algoritmos de classificação.
* Escolher o melhor modelo utilizando métricas robustas.
* Comunicar os resultados por meio de visualizações claras para stakeholders.

---

# 📂 Base de Dados

A base contém informações de partidas ranqueadas de League of Legends.

### Variável alvo

```
blueWins
```

* 1 → Time Azul venceu
* 0 → Time Vermelho venceu

### Exemplos de atributos

* Ouro total
* Experiência
* Torres destruídas
* Dragões
* Arautos
* Eliminações
* Assistências
* Diferenças entre os times (features `diff`)

---

# 🛠 Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* XGBoost

---

# 📊 Processo do Projeto

## 1. Carregamento dos dados

* Importação da base
* Inspeção inicial
* Tipos das variáveis
* Valores ausentes

---

## 2. Análise Exploratória (EDA)

Foi realizada uma análise completa para compreender o comportamento dos dados.

Incluindo:

* distribuição da variável alvo;
* correlação entre variáveis;
* estatísticas descritivas;
* identificação de possíveis redundâncias.

---

## 3. Engenharia de Atributos

Foram realizadas diversas melhorias na base:

* remoção de variáveis redundantes;
* criação das variáveis de diferença (`diff`);
* tratamento de valores ausentes;
* preparação dos dados para modelagem.

---

## 4. Modelos Testados

Foram avaliados diversos algoritmos de classificação.

* Regressão Logística
* Naive Bayes
* Árvore de Decisão
* Random Forest
* Gradient Boosting
* XGBoost
* Ensemble (Voting Classifier)

Além disso foi realizado:

* Validação Cruzada (Stratified K-Fold)
* RandomizedSearchCV para otimização de hiperparâmetros

---

# 📈 Métricas Avaliadas

Os modelos foram comparados utilizando:

* Acurácia
* Precisão
* Recall
* F1-Score
* ROC-AUC

A escolha do modelo final foi baseada principalmente no **ROC-AUC**, por ser uma métrica mais robusta para problemas de classificação.

---

# 📊 Visualizações

## Comparação dos Modelos (AUC)

![Comparação dos Modelos](images/auc.png)

## Curva ROC

## Matriz de Confusão

## Importância das Variáveis

## Heatmap de Correlação

## Distribuição da Variável Alvo

# 📌 Principais Insights

Após a análise foi possível observar que:

* as diferenças entre ouro, experiência e objetivos possuem forte influência no resultado da partida;
* estatísticas coletadas nos primeiros minutos já permitem prever o vencedor com boa precisão;
* modelos baseados em árvores apresentaram excelente desempenho;
* o ajuste de hiperparâmetros melhorou significativamente a capacidade preditiva do modelo.

---

# 🚀 Como Executar

Clone o repositório

```bash
git clone https://github.com/seuusuario/nome-do-projeto.git
```

Entre na pasta

```bash
cd nome-do-projeto
```

Instale as dependências

```bash
pip install -r requirements.txt
```

Execute o notebook

```bash
jupyter notebook
```


# 📁 Estrutura do Projeto

```
📦 projeto-lol

├── data/
│   └── base de dados.csv
│
├── notebooks/
│   └── Previsão de Vitória em Partidas Ranqueadas de League of Legends.ipynb
│
├── images/
│   ├── comparacao_auc.png
│   ├── curva_roc.png
│   ├── matriz_confusao.png
│   ├── importancia_variaveis.png
│   ├── heatmap.png
│   └── distribuicao_alvo.png
│
├── app.py
├── requirements.txt
└── README.md
```
# 👨‍💻 Autor

**Elias Ramineli**

Projeto desenvolvido como prática de Ciência de Dados e Machine Learning, aplicando técnicas de análise exploratória, engenharia de atributos, validação cruzada, otimização de hiperparâmetros e avaliação de modelos de classificação.

---

# ⭐ Se este projeto foi útil

Deixe uma ⭐ no repositório para apoiar o desenvolvimento de novos projetos.
