# 🎮 Previsão de Vitória em Partidas Ranqueadas de League of Legends

📌 Sobre o Projeto
Este projeto aplica técnicas de Ciência de Dados e Machine Learning para prever se o time azul vencerá uma partida ranqueada de League of Legends.
O trabalho foi desenvolvido seguindo um fluxo completo de um projeto de Data Science, desde a exploração dos dados até a comparação de modelos e otimização de desempenho.
________________________________________
🎯 Objetivo
Construir um modelo de classificação capaz de prever o resultado de uma partida utilizando apenas informações estatísticas da fase inicial do jogo.
________________________________________
📂 Base de Dados
A base contém estatísticas das partidas ranqueadas, incluindo informações dos dois times, como:
•	Ouro obtido
•	Experiência
•	Abates
•	Torres destruídas
•	Dragões
•	Arautos
•	Barões
•	Minions
•	Nível médio
•	Diversas outras métricas da partida
A variável alvo do projeto é:
blueWins
•	1 → Vitória do Time Azul
•	0 → Vitória do Time Vermelho
________________________________________
🔍 Etapas do Projeto
1. Entendimento dos Dados
•	Análise das variáveis
•	Estatísticas descritivas
•	Identificação de valores ausentes
•	Compreensão da variável alvo
________________________________________
2. Análise Exploratória (EDA)
Foram desenvolvidas diversas visualizações para compreender melhor os dados.
Entre elas:
•	Distribuição da variável alvo
•	Histogramas
•	Boxplots
•	Heatmap de correlação
•	Comparação entre variáveis
•	Análise estatística das principais métricas
________________________________________
3. Engenharia de Atributos
Nesta etapa foram realizadas melhorias importantes na base de dados:
•	Remoção da coluna gameId
•	Tratamento de valores ausentes
•	Redução de redundâncias
•	Criação de variáveis de diferença (diff) entre os dois times
Essas transformações permitiram representar melhor o equilíbrio entre as equipes e melhorar a capacidade preditiva dos modelos.
________________________________________
4. Modelagem
Foram comparados diferentes algoritmos de classificação:
•	Regressão Logística
•	Árvore de Decisão
•	Random Forest
•	Gradient Boosting
Após a comparação inicial, foi realizado ajuste de hiperparâmetros utilizando RandomizedSearchCV para otimizar o modelo de melhor desempenho.
________________________________________
5. Avaliação dos Modelos
Os modelos foram avaliados utilizando métricas amplamente empregadas em projetos profissionais:
•	Acurácia
•	Precisão
•	Recall
•	F1-Score
•	ROC-AUC
•	Curva ROC
•	Matriz de Confusão
•	Validação Cruzada (Cross Validation)
A escolha do modelo final priorizou a métrica ROC-AUC, por representar melhor a capacidade do modelo em distinguir partidas vencedoras e perdedoras.
________________________________________
📊 Principais Visualizações
O projeto inclui gráficos para apoiar toda a análise:
•	Distribuição da variável alvo
•	Heatmap de correlação
•	Histogramas
•	Boxplots
•	Comparação entre modelos
•	Curva ROC
•	Matriz de Confusão
•	Importância das variáveis
________________________________________
🛠 Tecnologias Utilizadas
•	Python
•	Pandas
•	NumPy
•	Matplotlib
•	Scikit-learn
•	Gradient Boosting
•	Random Forest
•	RandomizedSearchCV
________________________________________
📈 Resultados
Após comparar diferentes algoritmos e realizar o ajuste de hiperparâmetros, foi selecionado o modelo com melhor capacidade de generalização.
A validação em dados nunca vistos demonstrou que o modelo consegue realizar previsões consistentes, apresentando excelente equilíbrio entre precisão, recall e capacidade de discriminação das classes.
________________________________________
💡 Principais Aprendizados
Durante o desenvolvimento deste projeto foi possível aplicar diversas etapas fundamentais da Ciência de Dados:
•	Exploração e interpretação de dados;
•	Engenharia de atributos;
•	Preparação e limpeza de dados;
•	Comparação entre algoritmos de Machine Learning;
•	Ajuste de hiperparâmetros;
•	Validação estatística;
•	Interpretação dos resultados.
________________________________________
👨‍💻 Autor
Elias da Silva Santos Filho
Projeto desenvolvido como prática de Ciência de Dados, aplicando técnicas de Machine Learning supervisionado para classificação e previsão de resultados em partidas de League of Legends.
________________________________________
⭐ Se este projeto foi útil para você, deixe uma estrela no repositório!
