#Análise de Qualidade de Vinhos com Random Forest#

🍷 Sobre o Projeto
O objetivo deste projeto foi desenvolver um modelo de classificação capaz de prever a nota de qualidade (quality) de vinhos tintos. Para isso, utilizei um conjunto de dados com variáveis físico-químicas e apliquei o algoritmo Random Forest em um cenário multiclasse.

📊 O que foi feito?
Preparação e Limpeza: Comecei pelo básico: entendi os tipos de dados e garanti que não houvesse valores ausentes que pudessem comprometer a análise.
Exploração dos Dados (EDA): Analisei como as variáveis se distribuem e, principalmente, como o alvo (quality) estava balanceado. Também identifiquei quais características químicas tinham maior correlação com a nota final.
Modelagem e Baseline: Separei os dados em treino e teste (usando stratify para manter a proporção das classes) e treinei um RandomForestClassifier como ponto de partida.
Otimização e Performance: Como o dataset é desbalanceado, não foquei apenas na acurácia. Usei técnicas de oversampling e realizei uma busca de hiperparâmetros via Random Search para encontrar o melhor equilíbrio entre as classes.
Validação: Avaliei o resultado final comparando o modelo otimizado com o baseline, utilizando matriz de confusão e métricas como F1-Score e Balanced Accuracy para garantir uma visão real do desempenho.

🛠️ Tecnologias Utilizadas
Manipulação: Pandas e Numpy
Machine Learning: Scikit-learn e Imbalanced-learn
Visualização: Matplotlib e Seaborn
